+++
date = '2026-03-10T16:33:28+08:00'
draft = true
title = 'Road to 30'
+++

# BLD Journey

## Preface

這篇文章主要會分享我從「能夠盲解」到「熟悉 3-style」一路以來的心得與紀錄，額外包含了進步到平均 30 秒前各階段所做的努力與一些心得，希望可以給想~跳入火坑~學習 3-sytle 的其他玩家動機與方向。

## Before Starting 3-style

### Why 3-style?

~因為很帥啊（X~

以下是認真的說明。
3-style 基本上可以視為現今盲解領域中能夠被人類實際掌握的解法中效率最高的，此處效率的定義指的是解出每個 target 所需要的「時間」。
相較於一次只能解一個 target 的 OP、Orozco、M2/R2 等初階解法，3-style 可以一次性的解好兩個 targets，同時也比 BH、3OP 等同樣為三循環的解法有更順手的轉法或更少步數。

至於一些在 3-style 之後的優化，如 Floating，則比較偏向針對相同的打亂設法降低 target 數，而非進一步縮短每個 target 所需的時間。
當然，LTCT 還是可以被歸類比 3-style 更進階、對 target 效率的優化。
但無論如何，3-style 都已經可以算是當前流行的進階盲解解法中最核心的部分。

約莫在 2025 年底時，我下定決心要認真練習盲解，並以 30 秒內做為目標。
理所當然學習 3-style 也成為了我這段路上的必修科目之一。

### My definition for full 3-style

首先，我想先定義一下我認知中完整掌握 3-sytle 解法所需要學會並能夠順暢使用的公式或技巧，另外說明一下我的 buffer 是 UFR 和 UF：

- Corner commutators：378 cases
- Edge commutators：440 cases
- UF-UR/buffer-any parity：21 cases
- buffer-any corner twist：14 cases
- buffer-any edge flip：11 cases

即使是最基本的要求，3-style 也需要學習總共 864 條「公式」。
我會說這並沒有大多數 CFOP 使用者想像的困難，畢竟極大部分都只是可推導的 commutators、公式之間也常共享類似的原理，要完全掌握並不是天方夜譚。
然而，3-style 中不同公式的 set-up 方式十分靈活，有時候最優的解法反而很反直覺。
如果沒有足夠的時間投入，要能夠在這麼多不同 cases 間靈活運用仍非易事。

因此，如果對盲解還沒有足夠的熱情與耐心，~M2/Orozco 很棒也足夠有趣了~。

### Something I knew before 3-style

好的，相信看到這兒的各位都決心要踏入 3-style 的世界了。
在正式開始我的學習歷程之前，我想再說說我在開始 3-sytle 之前的盲解程度與相關的事前準備。

我大概是在 1:40 左右開始學習 Corner 3-style、1:15 左右開始學習 Edge 3-style。
但我覺得 3-style 本來就是越早學越好，所以什麼程度開始學其實沒什麼決定性的結論，確定有動力想學就去學吧！
只要確保自己對盲解的概念完全熟悉，而且知道 commutator 是什麼就夠了。

另外是一些加分項，我認為不是必須但可以有效提升學習效率，也能在學習的同時維持練習和進步的節奏。

- 

## Main Course: About Learning 3-style

### Resources

這裡提供一些我覺得很不錯的 3-style 資源供參考，大家可以挑自己喜歡的看。
在公式表的部分我蠻推薦用 Jack Cai 的 beginner sheet 搭配 BLDDB，邊學邊整理出自己最順手的 3-style 公式。

### Learning order

我自己推薦的順序是先學 Corner 再學 Edge，其他的隨意，有學起來就好了。
會建議先學 Corner 的原因主要有二，一個是關於難度、另一個則是關於解法間的銜接。

普遍來說，我認為 Corner 3-style 雖然公式數目較少，但其難度平均而言仍大於 Edge 3-style，因此率先學習能夠預留更多的時間去熟悉它。




### Parity

Parity 比較沒有什麼技巧可言，比較需要在意的只有 set-up moves 和 PLL 公式間的消步，還有幾個非 PLL 公式的 target 而已。
~基本上在學習 3-style 的漫漫長河中~，21 條 Parity 公式可以說是相對簡單的部分了，時不時背一下複習一下，並在實戰中試著使用就可以輕鬆學起來了。

### Twisted Corners & Flipped Edges



### Corner 3-style



### Edge 3-style




## After 3-style

### Practice

### One-pass Memorization

### Advanced techniques



## 正文

先說明我學習的 3-sytle 都是以 UF/UFR 作為 Buffer。
順序的部分，我自己是先學 Corner 再學 Edge，各花了大約 1 週半的時間學習、1 週的時間熟悉轉法。
會先選擇 Corner 的理由是我認為 M2 在初學階段已經足夠快速、且 Corner 3-style 與 Orozco 共用同個 buffer，能夠隨時互換，轉換上比較無痛。

當然，我也有聽說不少人是先從 Edge 開始學的，因為 Edge 的公式通常比較短。
不過我自己認為 Edge 用到的消步和手法實際上都比較困難，而且沒辦法與 M2 混用。
為了要在學習的同時保有練習的步調，以盲解項目整體的進步節奏去考量後，我最終還是選擇了從 Corner 開始。

但這其實就是個人喜好啦，反正最終都得要全部學會 XD。

### 開始學習的時機

這個問題很有趣，如果讀者最終的目標很明確，我認為在理解力可以負荷的情況下，3-style 是越早學越好。
正如同我們在速解上不會要求把 LBL 練到 sub 20 才開始學 CFOP 一樣，盲解也沒有什麼理由去限制自己一定要達到什麼成績才能學什麼解法。
而且 3-style 的熟悉相比 F2L 又需要更多的時間、心力，早點開始反而能避免轉換的陣痛與挫折感，我認為是有助於學習的成功率的。

### 教材

我主要是用 Jack Cai 的 3-sytle sheet 學習的，它以貼紙做分類我覺得蠻初學者友善的。
但我同時也認為 Jack 為初學者準備的 sheet 也包含了一些雖說好記但稍嫌不順手、不夠有效率的公式。
因此我也一併參考了 J perm 的 sheet 與 BLDDB 中羅列的轉法，修改成最適合自己的 3-style sheet。

### Corner 3-style

我自己就是一個貼紙一個貼紙學，由於有過使用 Orozco 的經驗，頂層的三張貼紙我大概花 2 天熟悉，剩下的 Commutator 大約是一天 1-2 張貼紙的進度，最後幾張會快很多，畢竟很多都只是前面的 inverse 而已。

我覺得一個好的學習方式是去注意不同 Commutator 之間的關聯性，舉例 UFR -> UBL -> DBR（\[R D' R':\[R' D R, U2\]\]）與 UFR -> UFL -> DBR（\[R D' R':\[R' D R, U'\]\]）就幾乎可以說是一樣的 setup 與 Commutator 類型。
雖然不是每組相似的 Commutator 都能像例子中的這麼好理解，但學習 3-style 本來就是需要花時間的，不要想一步登天，慢慢的去感受 Commutator 的直覺並建立公式之間的關係，我認為才是學好 3-style 的方法。
可能一開始學習時常會驚嘆這樣的轉法到底怎麼想出來的，然而越到後來反而會越能夠理解，甚至是可以自己想出最佳做法。

此外，我很建議學習的同時多做一些 Flashcard 與明解練習。
我自己在看完所有 case 之後，也是另外花了一週的時間隨機生成 Letter Pairs 來複習，也做了很多直接看著解的練習，才達到了足以實際使用的熟悉度。

總而言之，我總共花了 2 至 3 週才真正能在正式的盲解中使用 Corner 3-style，而不會總是想不起做法。
（註：如果讀者和我一樣原本使用 Orozco 的話，轉換的過程中如果忘記公式了依然可以換回 Orozco 用 2 條 Commutator 解完，不會因為忘記公式就得直接 DNF。）


### Edge 3-style

Edge 的學習途徑跟 Corner 差不多，都是一張貼紙一張貼紙來，並在過程中找關聯性。
比較不一樣的是 Edge 有很多 Mirror 的做法（因為 Buffer 位置有對稱性），算上 inverse 的話實際上只有 100 多種轉法而已，我認為學習難度確實是比 Corner 小的。
不過 Edge 的手法和消步上有不少特別的做法（例如 M + L 直接做成 Lw、該用 S 還是用 E 去 insert 的選擇），建議在學習的時候就可以稍微注重一下，真正換過去 3-style 時比較可以感受出效率上的優勢。

#### 4-Mover

Edge 有很多形如 \[M', U2\]、\[S, R2\]、\[E, R2\] 等俗稱 4-Movers 的換三邊轉法，要先做中間層或先做側面有時候蠻不直覺的。
好消息是這些轉法間都有個共通的守則，舉例 UF->FL->DR，我會先做 U' R' setup、inverse 就改成 U R；UF-BL->DR 的話則是 U' R setup、inverse 用 U' R'。
眼尖的讀者可以發現如果是中間層 target 在前的話，就要把 Buffer 往 Slice 的中間位置做 setup，反之則往邊緣放。
有這樣的認知大概九成的 4-Mover 方向都可以輕鬆掌握，只需要另外注意消步就好。

#### Edge-Only Solves



### Parity/Twist/Flip


## 後記

### 學習心得

### 練習

熟能生巧可以說是解方塊最重要的一句話了。
尤其 3-sytle 中動輒 800 多種不同的 case，自然也需要大量的練習才能行雲流水。
在學習完基本的 Full 3-style 之後，我認為最合適的下一步便是持續的使用它，讓一切轉法都變得足夠直覺、減少公式間的停頓。（當然，這裡也牽涉到一些記憶部分的練習。）

### 進階一點

這裡附上一些我認為可以和 3-style 一起學起來的進階技巧，可以在不會花太多努力的情況下稍稍提升解法效率：

- Parity twist
- Mutiple corner twist/edge flip
- Breaking into corner twist/edge flip

## 參考資料

這裡主要是提供一些我看過而且認為有幫助的資源，供讀者參考。










