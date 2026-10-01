# Blog Maintenance

## Layout

| Path | Purpose |
|---|---|
| `content/en/` | All pages. `_index.md` = homepage, `about.md`, `posts/`, `poems/`, `cubing/` |
| `config/_default/` | `hugo.toml` site, `params.toml` theme options, `languages.en.toml` title/author, `menus.en.toml` nav |
| `layouts/shortcodes/` | `featured-cards.html`, `resume-button.html` |
| `layouts/partials/author.html` | Theme override: portrait at 384px for the About page author block |
| `layouts/_default/single.html`, `layouts/partials/toc.html` | Theme overrides: TOC as a plain list on the right (≥768px). After a theme update, re-copy `single.html` and reapply the `.article-body` / `.toc-side` change |
| `assets/css/custom.css` | Extra CSS (Blowfish's Tailwind is precompiled; unknown classes do nothing) |
| `assets/img/` | `background.webp`, `author.jpg`, `favicon.svg` (source for the favicon set in `static/`; re-render at 16/32/48/180/192/512 after editing) |
| `assets/icons/` | Custom SVG icons (`wca.svg`) |
| `static/` | Served as-is at site root: `resume.pdf`, favicons |
| `themes/blowfish/` | Submodule. Never edit. Override by copying a file to the same path under `layouts/` |
| `public/` | Build output. Not committed |

URLs have no language prefix: `/posts/freshman/`, `/about/`.

## Dev loop

```sh
hugo server -D        # preview with drafts, auto-reload at http://localhost:1313/
hugo                  # clean build, read WARN/ERROR lines
git add -A && git commit -m "..." && git push   # GitHub Actions deploys main
```

## New post

```sh
hugo new content/en/posts/my-slug/index.md    # or poems/, cubing/
```

- Set `draft = false` to publish.
- Feature image: put `featured.webp` in the post folder. Resize first:
  `cwebp -q 72 -resize 2000 0 in.png -o featured.webp`
- Tags in use: `Essay`, `Poetry`, `BLD`.

## Homepage featured cards

`content/en/_index.md`:

```markdown
{{< featured-cards "/posts/freshman" "/poems/darkblue" >}}
```

Paths without trailing slash. 3 per row (`assets/css/custom.css` → `.featured-cards`).

## About page

`content/en/about.md`. Replace `[...]` placeholders. Entry format:

```markdown
{{< timelineItem icon="graduation-cap" header="School" badge="2024 – now" subheader="Degree" md=true >}}
- bullet
{{< /timelineItem >}}
```

Icons: any name in `assets/icons/` or `themes/blowfish/assets/icons/` without `.svg`.

## Resume

1. Save as `static/resume.pdf` (< 1 MB).
2. `git add static/resume.pdf`, commit, push.
3. Button appears automatically; missing file = hidden button + build WARN.
4. Other name/label: `{{< resume-button file="cv.pdf" label="CV" >}}`

## Where to change what

1. Theme behaviour → `config/_default/params.toml`
2. Styling → `assets/css/custom.css`
3. New block inside content → `layouts/shortcodes/`
4. Change a theme element everywhere → copy partial from `themes/blowfish/layouts/partials/` to `layouts/partials/`, edit copy

Find a theme file: `grep -rn "text or class" themes/blowfish/layouts`

## Theme update

```sh
git submodule update --remote themes/blowfish
hugo server          # check, especially copied partials
git add themes/blowfish && git commit -m "update blowfish"
```

## Images

- Background: ~1920 px, < 600 KB, WebP. Served unresized.
- Post feature: ~2000 px, WebP/JPEG. PNG source → big PNG thumbnails.
- Unused large files in `assets/img/` (`background.png`, `pikachu.png`) are not published but bloat the repo.
