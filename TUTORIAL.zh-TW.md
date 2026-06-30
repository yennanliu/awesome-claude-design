# 新手教學：如何使用本倉庫（繁體中文）

> 🌐 語言：**繁體中文** ｜ 回到 [README.zh-TW.md](README.zh-TW.md) ｜ [English README](README.md)

這份教學帶你從零開始，學會如何使用 **Awesome Claude Design** 這個倉庫：找到適合的設計風格、把 `DESIGN.md` 套用到你自己的專案、用提示詞包與食譜加速，最後學會貢獻一份你自己的設計。

全程不需要先懂設計理論。你只需要：一個想做的專案（網站、app、簡報），以及 Claude Design 或 Claude Code 其中之一。

---

## 目錄

- [這個倉庫是什麼](#這個倉庫是什麼)
- [先搞懂三個名詞](#先搞懂三個名詞)
- [倉庫結構導覽](#倉庫結構導覽)
- [五分鐘快速上手](#五分鐘快速上手)
- [步驟一：挑一個美學家族](#步驟一挑一個美學家族)
- [步驟二：讀懂一份 DESIGN.md](#步驟二讀懂一份-designmd)
- [步驟三：把 DESIGN.md 套用到你的專案](#步驟三把-designmd-套用到你的專案)
- [步驟四：用提示詞包加速](#步驟四用提示詞包加速)
- [步驟五：用食譜走完整流程](#步驟五用食譜走完整流程)
- [進階：混搭兩個品牌](#進階混搭兩個品牌)
- [避開 AI 罐頭風](#避開-ai-罐頭風)
- [省 Token 的實用建議](#省-token-的實用建議)
- [貢獻一份你自己的 DESIGN.md](#貢獻一份你自己的-designmd)
- [常見問題](#常見問題)

---

## 這個倉庫是什麼

一句話：**一個按「視覺風格」分類的設計系統提示詞庫。**

每個檔案是一份 `DESIGN.md` — 一段結構化的設計規格（顏色、字體、元件、版面規則），你可以直接餵給 Claude Design 或 Claude Code，讓 AI 產出的介面有一致、不像罐頭的外觀。

本倉庫做的事：
- 把幾十個知名品牌的設計語言整理成可重用的 `DESIGN.md`
- 依「視覺性格」（編輯極簡、終端機核心、資料密集、電影感暗色……）分類，因為設計師就是這樣挑的
- 附上提示詞包（prompts）、端到端食譜（recipes）、混搭配方（remix）與反罐頭風工具

它不是什麼：不是 Claude Design 產品本身，也不是任何可下載的軟體。它是「素材與配方」。

---

## 先搞懂三個名詞

| 名詞 | 白話解釋 |
|---|---|
| **DESIGN.md** | 一份設計系統的「說明書」。用文字描述顏色（含十六進位色碼）、字體、按鈕長相、間距規則等。AI 讀了就知道該長成什麼樣子。 |
| **美學家族（family）** | 風格分類。例如「資料密集專業」適合儀表板，「趣味色彩」適合消費 app。本倉庫共 9 個家族。 |
| **SKILL.md** | 把一份 `DESIGN.md` 打包成「技能」，讓它能跨專案重複使用（進階用法）。 |

> 你 99% 的時間只會碰到 `DESIGN.md`。其他兩個先知道就好。

---

## 倉庫結構導覽

```
awesome-claude-design/
├── README.md              # 主目錄（英文）
├── README.zh-TW.md        # 主目錄（繁體中文）
├── TUTORIAL.zh-TW.md      # ← 你正在讀的這份
├── design-md/             # ★ 核心：所有 DESIGN.md，依家族分資料夾
│   ├── editorial/         #   編輯極簡
│   ├── terminal/          #   終端機核心
│   ├── warm/              #   暖色編輯
│   ├── data-dense/        #   資料密集專業（ClickHouse、CrewAI、Langfuse、FinLab…）
│   ├── cinematic/         #   電影感暗色
│   ├── playful/           #   趣味色彩（Figma、Toss、Grab…）
│   ├── glass/             #   玻璃／柔未來感
│   ├── brutalist/         #   霓虹粗獷
│   ├── indie/             #   小眾／獨立
│   └── remix/             #   混搭配方（兩個品牌結合）
├── prompts/               # 可直接複製貼上的提示詞包
├── recipes/               # 端到端工作流程（含步驟）
├── showcase/              # 用 Claude Design 做出的實際作品
└── assets/                # 預覽圖、標籤徽章、橫幅
```

最重要的資料夾是 **`design-md/`**。其餘都是輔助。

---

## 五分鐘快速上手

如果你只想趕快試一次，照這個做：

1. 打開 [README.zh-TW.md 的預覽藝廊](README.zh-TW.md#預覽藝廊)，看哪個縮圖最接近你想要的感覺。
2. 點該縮圖下方的圖說，開啟對應的 `DESIGN.md`。
3. 複製整份 `DESIGN.md` 的內容。
4. 在 Claude Design 或 Claude Code 中貼上，並加一句：
   > 「請依照以下這份 DESIGN.md 的設計系統，幫我做一個〔你的需求，例如：SaaS 產品的登陸頁〕。嚴格遵守裡面的顏色、字體與元件規則。」
5. 看結果。不滿意就用行內註解（在 Claude Design）或再追加一句話微調。

就這樣。下面是把每一步做好的細節。

---

## 步驟一：挑一個美學家族

不知道選哪個？回答三個問題（這也是 README 裡的「如何選擇家族」）：

1. **產品偏重閱讀，還是偏重掃視數據？**
   - 閱讀 → 編輯極簡 / 暖色編輯
   - 掃視 → 資料密集專業 / 終端機核心
2. **使用者是誰？**
   - 開發者 → 終端機核心 / 資料密集專業
   - 設計師、創作者 → 電影感暗色 / 趣味色彩
   - 一般消費者 → 玻璃／柔未來感 / 趣味色彩
3. **品牌需要「有膽量」、讓人記住嗎？**
   - 需要 → 霓虹粗獷 / 小眾獨立
   - 不需要 → 留在前面那些

挑好家族後，進對應資料夾（例如 `design-md/data-dense/`）瀏覽裡面的品牌，挑一個色票最對味的。

> 💡 也可以讓 AI 幫你挑：把 [`prompts/family-picker.md`](prompts/family-picker.md) 貼給 Claude，回答它的問題，它會推薦家族 + 兩份參考 `DESIGN.md`。

---

## 步驟二：讀懂一份 DESIGN.md

每份 `DESIGN.md` 結構幾乎一致。以資料密集家族的 `design-md/data-dense/crewai.md` 為例，常見章節：

| 章節 | 它在說什麼 | 你該注意 |
|---|---|---|
| 1. 視覺主題與氛圍 | 整體感覺、一句話定位 | 確認跟你的產品調性合 |
| 2. 色彩調色盤與角色 | 所有顏色 + 十六進位色碼 + 用途 | **最重要**，直接決定外觀 |
| 3. 字體規則 | 標題/內文/等寬字、字重、字級 | 換字體就能大改氣質 |
| 4. 元件樣式 | 按鈕、卡片、表格、輸入框長相 | 對照你需要的元件 |
| 5. 版面原則 | 網格、間距、側欄寬度 | 影響整體佈局 |
| 6. 深度與層次 | 陰影、邊框怎麼用 | 細節質感來源 |
| 7. Do's / Don'ts | 該做與不該做 | 餵給 AI 時最有效的約束 |
| 8. 響應式行為 | 手機/平板/桌面差異 | 多裝置時看這段 |
| 9/10. 國際化、Agent 提示指南 | 多語系、給 AI 的精煉指令 | 第 10 節常是「一段就能用」的濃縮版 |

**小技巧：** 大多數 `DESIGN.md` 的最後一節（例如「Agent Prompt Guide」/「Agent 提示指南」）是整份的濃縮。趕時間的話，光貼這一段也能用。

---

## 步驟三：把 DESIGN.md 套用到你的專案

### 情境 A — 在 Claude Design（網頁產品）

1. 開新專案，把整份 `DESIGN.md` 內容貼進對話。
2. 描述你要的東西（「一個記帳 app 的儀表板畫面」）。
3. 生成後，**用行內註解微調**，不要每次都開新對話（省額度，見後面）。

### 情境 B — 在 Claude Code（終端機/IDE）

1. 在你的專案根目錄建立一個 `DESIGN.md`，把選好的內容貼進去（可改成你的品牌色）。
2. 直接對 Claude Code 說：
   > 「讀取專案根目錄的 `DESIGN.md`，依它的設計系統實作〔某個頁面/元件〕。」
3. Claude Code 會把顏色變成 CSS 變數、依規格建元件。

### 共用要訣
- **先建系統，再做頁面。** 讓 AI 先確立 tokens，後面每個畫面才會一致。
- **明確引用規則。** 與其說「做漂亮一點」，不如說「用 `--accent` 當主按鈕色、卡片圓角 12px，依 DESIGN.md 第 4 節」。
- **改色就改 token。** 想換品牌色，只要改 `DESIGN.md` 裡的 `--accent` 等變數，其他規則照舊。

---

## 步驟四：用提示詞包加速

`prompts/` 裡每個 `.md` 都是「複製即用」的提示詞，附範例輸出。

| 提示詞包 | 什麼時候用 |
|---|---|
| [`brand-to-design-md.md`](prompts/brand-to-design-md.md) | 你有一個品牌網址，想自動生出一份 `DESIGN.md` |
| [`audit-live-site.md`](prompts/audit-live-site.md) | 想讓 AI 替現有網站打分數、列出改進清單 |
| [`3-designer-debate.md`](prompts/3-designer-debate.md) | 想要三位「設計師人格」互相辯論給更好建議 |
| [`remix-two-brands.md`](prompts/remix-two-brands.md) | 想把兩個品牌風格融合 |
| [`family-picker.md`](prompts/family-picker.md) | 不知道該選哪個家族 |
| [`break-default-aesthetic.md`](prompts/break-default-aesthetic.md) | 產出看起來很「AI 罐頭」，想打破預設 |

用法都一樣：打開檔案 → 複製提示詞 → 貼給 Claude → 按指示填空。

---

## 步驟五：用食譜走完整流程

`recipes/` 是端到端的完整流程，每個都有實際步驟。新手最推薦從這兩個開始：

- [**20 分鐘登陸頁**](recipes/landing-page-20-min.md)：DESIGN.md → Claude Design → Claude Code → 上線（Vercel）。最完整的「從零到上線」示範。
- [**現有倉庫 → 設計系統**](recipes/repo-to-design-system.md)：把 Claude 指向你既有的 CSS，反向抽出一份標準 `DESIGN.md`。

其他實用的：
- [**Figma 檔案 → DESIGN.md**](recipes/figma-to-design-md.md)
- [**從 README 做簡報**](recipes/pitch-deck-from-readme.md)
- [**Token 預算控制**](recipes/token-budget-claude-design.md)（強烈建議讀）

---

## 進階：混搭兩個品牌

單一品牌複製久了會無聊。`design-md/remix/` 收了現成的混搭配方，例如：

- **Linear × Claude** = Linear 的字體 + Claude 的陶土暖色 → 有靈魂的編輯型 SaaS
- **Warp × Sentry** = 終端機網格 + 淡紫紫 → 不冰冷的開發者儀表板

自己做：用 [`prompts/remix-two-brands.md`](prompts/remix-two-brands.md)，餵兩份 `DESIGN.md`，它會幫你仲裁 token 衝突（誰的顏色贏、誰的字體贏），產出一份合併版。

---

## 避開 AI 罐頭風

社群最大的抱怨：AI 產出的設計都長一樣（到處藍綠色、閃爍狀態點、三欄功能格……）。

最簡單的解法：把這段貼進你的系統提示詞或 `DESIGN.md` 開頭：

```
NEVER use generic AI-generated aesthetics:
- Overused font families (Inter, Roboto, Arial, system fonts)
- Cliched color schemes (purple gradients on white or dark backgrounds)
- Predictable layouts and component patterns
- Cookie-cutter design that lacks context-specific character

DO use:
- Unique fonts chosen for the brand, not defaults
- Cohesive colors and themes grounded in the product's story
- Animations for effects and micro-interactions
- Context-specific character in every component
```

更完整的「預設指紋 → 反制規則」對照表，見 [README.zh-TW.md 的反罐頭風工具包](README.zh-TW.md#claude-design-的預設指紋避開)。一鍵中和的提示詞在 [`prompts/break-default-aesthetic.md`](prompts/break-default-aesthetic.md)。

---

## 省 Token 的實用建議

Claude Design 的視覺 token 很貴（約文字的 3 倍），很多人「兩個提示就燒掉 95% 週額度」。實用守則：

1. **一次搭好設計系統**，別反覆重生成整套。
2. **參考截圖上限 4 張** — 每張圖都很貴。
3. **用行內註解迭代**，不要每次開新對話。
4. **做變體用分支**，不要一直在同一條線上來回。
5. **最後一次打包交給 Claude Code** 收尾。
6. **促銷額度先用掉**（會過期），把每週額度留給正式工作。

完整配方：[`recipes/token-budget-claude-design.md`](recipes/token-budget-claude-design.md)。

---

## 貢獻一份你自己的 DESIGN.md

想把一個品牌加進這個倉庫？流程其實很固定（本倉庫近期新增 CrewAI、Langfuse、Grab 就是照這個做的）：

### 1. 選定品牌與家族
看那個品牌的網站，判斷它屬於哪個家族。例如：
- 儀表板/數據工具 → `data-dense`
- 消費 app、活潑彩色 → `playful`
- 全黑、電影感大圖 → `cinematic`

### 2. 建立檔案
路徑慣例：`design-md/<家族>/<品牌>.md`，例如 `design-md/playful/grab.md`。

### 3. 照標準章節寫 DESIGN.md
最快的方式：複製同家族中一份既有檔案當骨架（例如想加一個 playful 品牌，就複製 `design-md/playful/toss.md`），再依目標品牌改寫每一節。務必：
- 用**真實的十六進位色碼**（去看該品牌官網取色）
- 描述它**最有代表性的元件**（例如資料工具就寫「表格 / 圖表」，消費 app 就寫「服務卡片 / 大圖」）
- 第 7 節寫清楚 Do's / Don'ts，第 10 節寫一段「Agent 提示指南」濃縮版

> 也可以用 [`prompts/brand-to-design-md.md`](prompts/brand-to-design-md.md) 讓 AI 先生一份草稿，你再校稿。

### 4. 在 README 三個地方掛上去
為了讓它被看見，更新（中英文 README 對應位置）：
1. **「已收錄範例」那一長串連結**裡加上你的檔案
2. **該家族的表格**加一列（品牌 / 色票 / 字體 / 外部連結）
3. **預覽藝廊**加一張卡片（需要一張首頁截圖，放進 `assets/previews/`）

並在 `assets/previews/ATTRIBUTION.md` 補一列截圖來源。

### 5. 發 PR
- 標題格式：`[family] brand — 一行價值`
- 內文：色票 + 字體 + 參考連結 + 可重現性備註
- 標準（來自 CONTRIBUTING）：**一個在職設計師或工程師，會在 48 小時內覺得這有用嗎？**

詳見 [CONTRIBUTING.md](CONTRIBUTING.md)。

---

## 常見問題

**Q：我一定要付費的 Claude Design 才能用這個倉庫嗎？**
不用。`DESIGN.md` 是純文字規格，貼給任何能讀文字的 AI 工具都有用 — 包含 Claude Code、甚至其他模型。Claude Design 只是其中一個最順的搭配。

**Q：我可以直接拿這些品牌的設計來做商業產品嗎？**
這些 `DESIGN.md` 是用作**教育性參考**，描述公開可見的設計語言。品牌名稱與商標屬於各自所有者。請把它當作「學習風格的起點」，把顏色/字體換成你自己的品牌，不要原樣冒用他人商標。

**Q：DESIGN.md 要全部貼，還是貼一部分？**
理想是全貼。趕時間可只貼第 2 節（顏色）+ 第 10 節（Agent 提示指南）。

**Q：產出的東西還是很「AI」，怎麼辦？**
先套用[反罐頭風工具包](#避開-ai-罐頭風)，再在提示詞裡明確指定品牌專屬的字體與強調色（不要用預設的 Inter + 藍綠色）。

**Q：我想加的品牌已經有人收錄了，怎麼辦？**
可以做**混搭版**（remix），或補充一個不同家族的詮釋。重複原樣的條目會被婉拒。

---

<p align="center">
  有問題或想補充？歡迎開 issue 或 PR。回到 <a href="README.zh-TW.md">繁體中文 README</a>。
</p>
