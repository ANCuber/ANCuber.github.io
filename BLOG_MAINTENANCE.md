# Blog Maintenance

This guide covers the homepage featured links and creating posts for this Hugo blog.

## Homepage featured links

Edit `content/_index.md`. Add a post path to the `featured-cards` shortcode to show it as a Blowfish card. For example:

```markdown
## 精選文章

{{< featured-cards "/zh-tw/posts/freshman" "/zh-tw/cubing/bld-resources" >}}
```

Use each post's Hugo content path without a trailing slash. In this site build, Chinese pages use the `/zh-tw/` prefix. Remove an argument to unfeature a post. Cards use each post's feature/cover/thumbnail image when available and are independent of post dates.

## Create a post

From the repository root, create a page bundle with a URL-friendly folder name:

```sh
hugo new content/zh-tw/posts/my-post/index.md
```

Replace `my-post` with a short slug. Hugo creates the post from `archetypes/default.md`. Add images for the post to the same folder and reference them with page-relative paths where appropriate.

Preview the site locally, including drafts, with:

```sh
hugo server -D
```

Open the local address printed by Hugo. The GitHub Pages workflow publishes the site when changes are pushed to `main`; draft posts remain unpublished.