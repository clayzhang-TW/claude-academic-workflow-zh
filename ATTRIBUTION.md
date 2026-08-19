# 出處

書裡有一部分內容是從我自己的技能檔挖出來再改寫的——附錄 F 的十二個設計模式、附錄 H 的中文 AI 腔清單、附錄 I 的自審檢查表，還有正文幾節的判準。

那些技能檔有幾個本身改自公開專案。所以血緣是兩段：公開專案 → 我的技能檔 → 這本書。這一頁列出前面那一段。

## 本書的授權

CC BY-NC-SA 4.0。可以用，請註明出處；不可作商業用途；改編後散布須用同一授權。

## 上游對照

讀法：書的哪一節，用了我的哪一個技能，那個技能改自誰，什麼授權。

| 書中位置 | 我的技能 | 上游 | 授權 |
|---|---|---|---|
| 附錄 H 全份 | 中文潤稿技能 | [Raymondhou0917/speak-human-tw](https://github.com/Raymondhou0917/speak-human-tw)（雷蒙／侯智薰） | MIT |
| 7.1、詞彙表、附錄 I 的「保護片段」 | 同上 | [MrGeDiao/shuorenhua](https://github.com/MrGeDiao/shuorenhua) | MIT |
| **6.3 寫作模式鏈與 `[MATERIAL GAP]`；7.1 修稿模式；7.2 五角色自審；7.3 爆炸半徑檢查、唯讀稽核；附錄 I** | 論文寫作、審查與審查回應技能 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)（Cheng-I Wu）；[HKUSTDial/Supervisor-Skills](https://github.com/HKUSTDial/Supervisor-Skills) | **CC BY-NC 4.0**（見下節）；CC BY-NC-SA 4.0 |
| 7.1 逆向大綱、主張與證據對照 | 論文審查技能 | [Master-cai/Research-Paper-Writing-Skills](https://github.com/Master-cai/Research-Paper-Writing-Skills)，內容源自彭思達的公開筆記 | 見下節 |
| 4.1 五維度評分、三角色對抗 | 研究構想評估技能 | HKUSTDial/Supervisor-Skills 的 `idea-evaluator` | CC BY-NC-SA 4.0 |
| 4.1 三取向、四世界觀、三種效度 | 研究設計技能 | Creswell, J. W., & Creswell, J. D. (2018). *Research design* (5th ed.). SAGE. | 教科書，僅用其框架結構 |
| 2.4 執行前追問 | 執行前追問技能 | [mattpocock/skills](https://github.com/mattpocock/skills) 的 `grill-me`（Matt Pocock）；Anthropic〈[A field guide to Claude Fable 5: Finding your unknowns](https://claude.com/blog/a-field-guide-to-claude-fable-finding-your-unknowns)〉（Thariq Shihipar, 2026） | MIT；官方部落格，僅用其四象限框架 |
| 6.2 把一本書變成顧問 | 書轉技能的工具 | virgiliojr94，`book-to-skill` | MIT |

以下沒有上游，是我自己從零寫的：

| 書中位置 | 我的技能 |
|---|---|
| 3.2 貼出來的那份真實技能檔；5.1 存在查核 | 引用查核技能 |
| 4.3 檢索的五條工序、取用政策三條硬界線 | 文獻檢索技能 |
| 附錄 F 十二個設計模式 | 不是單一技能，是橫向掃過整套技能庫抽出來的 |
| 附錄 G 寫作聲紋 | 同上，來自對一批寫作技能的量測 |
| 本書的電子書排版 | 中文電子書排版技能 |

## Academic Research Skills：用得最多的一個上游

書裡有四處往上追到同一個地方：Cheng-I Wu 的 [Academic Research Skills](https://github.com/Imbad0202/academic-research-skills)（以下簡稱 ARS）。它是本書用得最多的單一上游，所以單獨一節說清楚。

**它要求的署名格式，原文如下：**

```
Based on Academic Research Skills by Cheng-I Wu
https://github.com/Imbad0202/academic-research-skills
```

授權 **CC BY-NC 4.0**：可自由使用與改編，須註明出處，不可作商業用途。本書的 CC BY-NC-SA 與它相容。

### 它有什麼

ARS 是四套給研究者用的技能，規模比本書用到的大很多：

| ARS 的套件 | 規模 |
|---|---|
| 論文寫作（Academic Paper） | 12 個角色、11 種模式 |
| 論文審查（Academic Paper Reviewer） | 7 個角色、6 種模式 |
| 文獻探索（Deep Research） | 13 個角色、8 種模式 |
| 全流程協調（Academic Pipeline） | 10 個階段 |

### 我改了什麼

**最大的改動不是砍項目，是換使用者。**

ARS 假設你會操作技能檔、會讓多個角色並行、會管理階段之間的交接。本書假設你**沒寫過程式**，而且是一個人在一個對話視窗裡工作。所以每一處的改動方向都一樣：**把多角色系統降維成一個人照著走的流程。**

| 書中位置 | ARS 原本 | 本書改成 | 為什麼 |
|---|---|---|---|
| **6.3 寫作模式鏈** | 11 種模式（含 `lit-review`、`format-convert`、`citation-check`、`disclosure` 等） | **6 種**：plan／outline／draft／revise／abstract／revision-coach | 砍掉的五種要嘛在本書別章已經處理（引用查核在第 5 章、使用聲明在附錄 D），要嘛對初學者是額外負擔。⚠️ 另外**加了 `draft`**——ARS 把撰寫包在 `full` 裡，但本書要單獨標出它，因為那是唯一「它可能替你生出東西」的一格 |
| **7.2 五角色自審** | 7 個審查角色 | **5 個**：主編／方法論／領域／視角／魔鬼代言人 | 砍掉兩個偏格式與統計細節的角色，它們的工作在 7.1 第三輪與附錄 I 各自處理。⚠️ 並改為**分五次對話跑**，因為讀者沒有多角色並行的環境——這個限制反而讓「五個角色互相不知道」變成必然而不是設定 |
| **附錄 I** | 6 種審查模式、0–100 評分量尺 | **不收模式、不收量尺**，只收八個品質面向與五條拒稿標準 | 評分量尺是模擬審查者給分用的，對自審讀者會誘發「我幾分」這種錯問題。⚠️ 五條拒稿標準改寫為**教育測量取向**（樣本數、測量恆等性、效度來源），與 ARS 原本的領域不同 |
| **7.1 修稿** | `revision` 模式 | **拆成三輪**（邏輯 → 去 AI 腔 → 格式），並規定同一對話跑完 | 一次要它全部處理，等於把 ARS 拆開的東西又壓回去 |
| **文獻探索** | 13 個角色、8 種模式 | **幾乎沒用** | 第 4 章的檢索工序來自另一套來源。ARS 這一塊對初學者太重 |
| **十階段全流程** | 10 個階段的協調器 | **完全沒用** | 本書的七章本身就是那個順序，再套一層協調器只會多一層抽象 |

### 一件值得說的事

⚠️ **第 3 章 3.5 說「不要硬搬別人的技能」，理由是四條：跳過發現摩擦、繼承別人的品質標準、拿到查不動的黑箱、領域不通用。**

上面那張表就是我自己照那四條做了一次。ARS 的模式我用了六個、砍了五個，砍的判準不是「這個功能不好」，是**「本書的讀者這一週會不會用到」**。那個判準只有我知道，因為只有我知道我的讀者是誰。

**你拿本書的東西去用的時候，該做同一件事。**

---

## 彭思達的研究筆記

7.1 的逆向大綱與「主張—證據對照」，往上追是：我的論文審查技能 ← Master-cai/Research-Paper-Writing-Skills（MIT）← 彭思達（Peng Sida）的公開研究筆記。

Master-cai 的 README 寫明該 repo 的貢獻是「整理、結構化改寫、封裝成可重用的技能」，寫作知識與方法論本身來自彭思達的公開筆記。那個 MIT 授的是封裝那一層。

彭思達的原始 repo 沒有授權宣告，預設狀態是著作權全部保留，但作者在文件裡寫了條件：

> 如果轉載該文檔的內容，請註明出處：https://github.com/pengsida/learning_research

本書照辦，出處與連結見上。

⚠️ 他的文件開頭另外聲明那些內容是為特定實驗室與他自己的科研經歷寫的。本書取用的是逆向大綱與主張—證據對齊兩項通用寫作紀律，已改寫為教育測量取向；它們在原始脈絡裡是為另一個領域寫的，用的時候要自己折算。

## 這些是怎麼確認的

表裡每一筆授權都開過上游 repo 本身核實，不是照抄我技能檔裡寫的宣告。兩個例外是 Creswell 那本教科書（實體書，引用的是框架結構，未逐頁讀過）與 Anthropic 那篇（官方部落格，讀過該頁）。

強調這件事，是因為技能檔裡的二手宣告出過錯，而且三次的方向不同：

- 我的技能檔寫附錄 I「整合自 Supervisor-Skills `handbook 1.1`」。開原檔之後，那份全文只有兩千多個位元組，內容是資料庫領域取向的「審稿人希望看到／討厭看到」各四條，原文寫著 `within the DB community`，附錄 I 一條都沒用到。⚠️ 不查的話，這本書會登記一筆它其實沒有的 CC BY-NC-SA 義務。
- 五維度評分同理。上游是 Higher／Faster／Stronger／Cheaper／Broader、十分制；本書是理論缺口／方法設計／樣本可行／測量嚴謹／實務貢獻、五分制。只有「用五個維度打分」這個形式相同，而形式不受著作權保護。
- 反方向的一次：我原本把四個中文潤稿專案都列成附錄 H 的上游，逐檔追下去才發現附錄 H 只用到其中一個。同一次比對也追出彭思達那一筆原本漏了。

多列會白白放棄授權選項，漏列會欠人一個交代，兩種都出現過。

## 不在這一頁的

- 文獻引用在各章〈延伸資源〉，每一筆附驗證層級
- AI Fluency 框架（4D）的授權與處理方式寫在第 4 章該節與其延伸資源
- 軟體與工具不列在這裡，它們是工具不是內容

---
