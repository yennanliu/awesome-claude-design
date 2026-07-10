# Awesome Claude Design（繁體中文版）

> 🌐 語言：**繁體中文** ｜ [English](README.md) ｜ 📘 新手教學：[TUTORIAL.zh-TW.md](TUTORIAL.zh-TW.md)

> **Claude Design** — Anthropic Labs 的 AI 設計工作空間。本倉庫依「美學家族」整理 DESIGN.md 檔案、混搭配方、附範例輸出的提示詞包、技能（skills）、影片拆解，以及發布週的社群動態。

<p align="center">
  <img src="assets/banner.svg" width="100%" alt="Awesome Claude Design — DESIGN.md prompts, skills, cookbooks, teardowns, remix recipes">
</p>

<p align="center">
  <img src="assets/mascot-dance.svg" width="320" alt="Dancing palette-knight mascot">
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <a href="https://github.com/rohitg00/awesome-claude-design/stargazers"><img src="https://img.shields.io/github/stars/rohitg00/awesome-claude-design?style=flat-square&logo=github&color=c96442" alt="Stars"></a>
  <a href="https://github.com/rohitg00/awesome-claude-design/network/members"><img src="https://img.shields.io/github/forks/rohitg00/awesome-claude-design?style=flat-square&logo=github&color=c96442" alt="Forks"></a>
  <a href="https://github.com/rohitg00/awesome-claude-design/commits/main"><img src="https://img.shields.io/github/last-commit/rohitg00/awesome-claude-design?style=flat-square&color=191817" alt="Last commit"></a>
  <a href="https://www.anthropic.com/news/claude-design-anthropic-labs"><img src="https://img.shields.io/badge/Launched-April%2017%2C%202026-0f0f0f?style=flat-square" alt="Launched"></a>
  <a href="https://www.anthropic.com"><img src="https://img.shields.io/badge/Opus-4.7-6f4e37?style=flat-square" alt="Opus 4.7"></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/rohitg00/awesome-claude-design?style=flat-square&color=blue" alt="License"></a>
</p>

<p align="center">
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-editorial.svg" alt="editorial minimalism"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-terminal.svg" alt="terminal-core"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-warm.svg" alt="warm editorial"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-data-dense.svg" alt="data-dense pro"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-cinematic.svg" alt="cinematic dark"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-playful.svg" alt="playful color"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-glass.svg" alt="glass / soft-futurism"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-brutalist.svg" alt="neon brutalist"></a>
  <a href="#各美學家族的-designmd"><img src="assets/tags/family-indie.svg" alt="cult · indie picks"></a>
</p>

Claude Design 於 **2026 年 4 月 17 日** 發布。同一天 Figma 股價收跌 **−4.26%**。YouTube 上的反應分成兩派：「前端工程師 RIP」與「又一個浪費 token 的爛功能」。本倉庫把兩派的聲音都收進來。

> **注意 — 假冒倉庫警告。** 一個名為 `anthropic-claude-design/claude-design`、宣稱可以「下載 Claude Design」的倉庫**並非** Anthropic 官方，也與其無任何關聯。真正的產品在 [claude.ai/design](https://claude.ai/design)，需透過 Pro/Max/Team/Enterprise 登入。沒有任何「下載」存在。請檢舉該假冒倉庫。

## 預覽藝廊

每個美學家族在實際產品中長什麼樣子。縮圖為各家族其中一個代表品牌的公開首頁靜態截圖。點圖片開啟線上網站，點圖說開啟本倉庫中可用的 `DESIGN.md`。

<table>
<tr>
<td align="center" width="33%">
<a href="https://linear.app"><img src="assets/previews/linear.jpg" width="100%" alt="Linear — editorial minimalism"></a><br>
<sub><b><a href="design-md/editorial/linear.md">Linear · editorial</a></b><br><code>#fff / #0f0f14 / #5e6ad2</code></sub>
</td>
<td align="center" width="33%">
<a href="https://ollama.com"><img src="assets/previews/ollama.jpg" width="100%" alt="Ollama — terminal-core"></a><br>
<sub><b><a href="design-md/terminal/ollama.md">Ollama · terminal</a></b><br><code>#000 / #fff / mono</code></sub>
</td>
<td align="center" width="33%">
<a href="https://www.anthropic.com"><img src="assets/previews/anthropic.jpg" width="100%" alt="Anthropic / Claude — warm editorial"></a><br>
<sub><b><a href="design-md/warm/claude.md">Claude · warm</a></b><br><code>#f4f3ee / #c96442 / #191817</code></sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
<a href="https://clickhouse.com"><img src="assets/previews/clickhouse.jpg" width="100%" alt="ClickHouse — data-dense pro"></a><br>
<sub><b><a href="design-md/data-dense/clickhouse.md">ClickHouse · data-dense</a></b><br><code>#181818 / #faff69 / magenta</code></sub>
</td>
<td align="center" width="33%">
<a href="https://crewai.com"><img src="assets/previews/crewai.jpg" width="100%" alt="CrewAI — data-dense pro"></a><br>
<sub><b><a href="design-md/data-dense/crewai.md">CrewAI · data-dense</a></b><br><code>#0b0e14 / #ff5e4d / ok #2dd4a7 / fail #f0506a</code></sub>
</td>
<td align="center" width="33%">
<a href="https://langfuse.com"><img src="assets/previews/langfuse.jpg" width="100%" alt="Langfuse — data-dense pro"></a><br>
<sub><b><a href="design-md/data-dense/langfuse.md">Langfuse · data-dense</a></b><br><code>#f6f5ef / #0a0a0a / highlight #f5f56b</code></sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
<a href="https://finlab.finance"><img src="assets/previews/finlab.png" width="100%" alt="FinLab — data-dense pro"></a><br>
<sub><b><a href="design-md/data-dense/finlab.md">FinLab · data-dense</a></b><br><code>#fff / #2563eb / gain #16a34a / loss #dc2626</code></sub>
</td>
<td align="center" width="33%">
<a href="https://runwayml.com"><img src="assets/previews/runwayml.jpg" width="100%" alt="RunwayML — cinematic dark"></a><br>
<sub><b><a href="design-md/cinematic/runway.md">Runway · cinematic</a></b><br><code>#000 / magenta + cyan</code></sub>
</td>
<td align="center" width="33%">
<a href="https://www.figma.com"><img src="assets/previews/figma.jpg" width="100%" alt="Figma — playful color"></a><br>
<sub><b><a href="design-md/playful/figma.md">Figma · playful</a></b><br><code>#0acf83 / #f24e1e / #a259ff</code></sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
<a href="https://arc.net"><img src="assets/previews/arc.jpg" width="100%" alt="Arc Browser — glass / soft-futurism"></a><br>
<sub><b><a href="design-md/glass/arc.md">Arc · glass</a></b><br><code>#fff / radial pastel</code></sub>
</td>
<td align="center" width="33%">
<a href="https://www.theverge.com"><img src="assets/previews/theverge.jpg" width="100%" alt="The Verge — neon brutalist"></a><br>
<sub><b><a href="design-md/brutalist/the-verge.md">The Verge · brutalist</a></b><br><code>#ff6600 / #000 / #fff</code></sub>
</td>
<td align="center" width="33%">
<a href="https://www.granola.ai"><img src="assets/previews/granola.jpg" width="100%" alt="Granola — cult / indie"></a><br>
<sub><b><a href="design-md/indie/granola.md">Granola · indie</a></b><br><code>#faf8f2 / warm glass</code></sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
<a href="https://www.grab.com/sg/"><img src="assets/previews/grab.jpg" width="100%" alt="Grab — playful superapp"></a><br>
<sub><b><a href="design-md/playful/grab.md">Grab · playful</a></b><br><code>#fff / #00b14f / #00692e</code></sub>
</td>
<td align="center" width="33%">
<a href="https://slima.ai/zh-TW"><img src="assets/previews/slima.jpg" width="100%" alt="Slima — warm editorial / literary"></a><br>
<sub><b><a href="design-md/warm/slima.md">Slima · warm</a></b><br><code>#faf9f6 / serif / amber+green+indigo</code></sub>
</td>
</tr>
</table>

<sub>截圖為公開首頁的靜態畫面，僅作編輯參考用途。商標權利皆歸各品牌所有者所有。來源網址與更新政策請見 <a href="assets/previews/ATTRIBUTION.md">ATTRIBUTION.md</a>。</sub>

## 目錄

- [預覽藝廊](#預覽藝廊)
- [認識 Claude Design](#認識-claude-design)
- [影片拆解](#影片拆解)
- [工具比較](#工具比較)
- [作品展示](#作品展示)
- [社群觀點](#社群觀點)
- [功能地圖](#功能地圖)
- [發布時間軸](#發布時間軸)
- [額度與 Token 預算](#額度與-token-預算)
- [官方資源](#官方資源)
- [X 訊號](#x-訊號)
- [各美學家族的 DESIGN.md](#各美學家族的-designmd)
- [混搭配方 Remix](#混搭配方-remix)
- [如何選擇家族](#如何選擇家族)
- [提示詞與食譜](#提示詞與食譜)
- [反罐頭風工具包](#反罐頭風工具包) — 包含 [Claude Design 的預設指紋](#claude-design-的預設指紋避開)
- [技能與外掛](#技能與外掛)
- [整合](#整合)
- [工作流程與食譜](#工作流程與食譜)
- [長篇教學](#長篇教學)
- [國際報導](#國際報導)
- [訣竅與技巧](#訣竅與技巧)
- [Podcast 報導](#podcast-報導)
- [常見問題](#常見問題)
- [相關開源專案](#相關開源專案)
- [標籤系統](#標籤系統)
- [參與貢獻](#參與貢獻)
- [授權](#授權)

---

## 認識 Claude Design

Anthropic Labs 的產品。把「對話」轉成「成品」的循環，用於原型、設計系統、簡報、單頁文件、登陸頁、行銷圖、品牌影片。由 **Claude Opus 4.7**（視覺模型）驅動。目前在 **Pro、Max、Team、Enterprise** 方案上以研究預覽（research preview）形式推出，發布當天逐步開放。

三大介面：
- **原型（Prototypes）** — 來源可以是文字、截圖、Figma `.fig`、倉庫 URL，或抓取的線上網站
- **設計系統（Design systems）** — 透過 `DESIGN.md` 為每個專案持久保存 tokens／元件；一個團隊可同時擁有多套
- **行銷素材（Collateral）** — 簡報、行銷頁、輪播圖、一次性貼文、品牌影片

## 影片拆解

點擊縮圖觀看。觀看次數透過 shields.io 即時更新。

<table>
<tr>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=IkspcJdeP3U"><img src="https://img.youtube.com/vi/IkspcJdeP3U/mqdefault.jpg" width="220"></a><br>
<b>Malewicz</b><br>
<img src="https://img.shields.io/youtube/views/IkspcJdeP3U?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/IkspcJdeP3U?style=flat-square&label=likes&color=c96442"><br>
<sub>資深設計師的質疑式拆解</sub>
</td>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=o4jIKc_DIoM"><img src="https://img.youtube.com/vi/o4jIKc_DIoM/mqdefault.jpg" width="220"></a><br>
<b>02ui · Murat Bayral</b><br>
<img src="https://img.shields.io/youtube/views/o4jIKc_DIoM?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/o4jIKc_DIoM?style=flat-square&label=likes&color=c96442"><br>
<sub>與 Lovable 正面對決</sub>
</td>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=uhQfErAzdiA"><img src="https://img.youtube.com/vi/uhQfErAzdiA/mqdefault.jpg" width="220"></a><br>
<b>WorldofAI</b><br>
<img src="https://img.shields.io/youtube/views/uhQfErAzdiA?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/uhQfErAzdiA?style=flat-square&label=likes&color=c96442"><br>
<sub>熱度導覽</sub>
</td>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=Qct36RA3y9k"><img src="https://img.youtube.com/vi/Qct36RA3y9k/mqdefault.jpg" width="220"></a><br>
<b>Ray Fernando</b><br>
<img src="https://img.shields.io/youtube/views/Qct36RA3y9k?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/Qct36RA3y9k?style=flat-square&label=likes&color=c96442"><br>
<sub>部落格即時改版</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=A2eEv3KYGPg"><img src="https://img.youtube.com/vi/A2eEv3KYGPg/mqdefault.jpg" width="220"></a><br>
<b>Vivek Mishra</b><br>
<img src="https://img.shields.io/youtube/views/A2eEv3KYGPg?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/A2eEv3KYGPg?style=flat-square&label=likes&color=c96442"><br>
<sub>發布日導覽</sub>
</td>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=4q2F4zblOLQ"><img src="https://img.youtube.com/vi/4q2F4zblOLQ/mqdefault.jpg" width="220"></a><br>
<b>AI for Work</b><br>
<img src="https://img.shields.io/youtube/views/4q2F4zblOLQ?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/4q2F4zblOLQ?style=flat-square&label=likes&color=c96442"><br>
<sub>從提示詞生出整套系統</sub>
</td>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=vyLaimDeK_g"><img src="https://img.youtube.com/vi/vyLaimDeK_g/mqdefault.jpg" width="220"></a><br>
<b>Greg Isenberg</b><br>
<img src="https://img.shields.io/youtube/views/vyLaimDeK_g?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/vyLaimDeK_g?style=flat-square&label=likes&color=c96442"><br>
<sub>實測它的邊界</sub>
</td>
<td align="center" width="25%">
<a href="https://www.youtube.com/watch?v=Hcvkc1XUhMg"><img src="https://img.youtube.com/vi/Hcvkc1XUhMg/mqdefault.jpg" width="220"></a><br>
<b>Ramanpal Singh</b><br>
<img src="https://img.shields.io/youtube/views/Hcvkc1XUhMg?style=flat-square&label=views&color=191817"> <img src="https://img.shields.io/youtube/likes/Hcvkc1XUhMg?style=flat-square&label=likes&color=c96442"><br>
<sub>新手教學</sub>
</td>
</tr>
</table>

## 工具比較

| 功能 | Claude Design | [Figma Make](https://www.figma.com/make) | [Lovable](https://lovable.dev) | [v0](https://v0.dev) | [Stitch](https://stitch.withgoogle.com) | [SuperDesign](https://github.com/superdesigndev/superdesign) |
|---|---|---|---|---|---|---|
| 提示詞 → 高保真 | 是 | 是 | 是 | 是 | 是 | 是 |
| 原生支援 DESIGN.md | **是** | 否 | 部分 | 否 | 首創 | 是 |
| 截圖 → 設計系統 | 是 | 否 | 部分 | 否 | 是 | 是 |
| 匯入 Figma `.fig` | 是 | 原生 | 是 | 部分 | 否 | 否 |
| 在線上網站做網頁擷取 | **原生** | 否 | 部分 | 否 | 否 | 部分 |
| 行內註解／調整旋鈕 | **是** | 是 | 否 | 否 | 否 | 否 |
| 每專案持久 tokens | **是** | 是 | 部分 | 否 | 否 | 是 |
| 組織範圍協作＋群組聊天 | **是** | 是 | 否 | 否 | 否 | 否 |
| 匯出路徑 | Canva/PDF/PPTX/HTML | Figma | 全端 app | React | HTML | 本地檔案 |
| 一個團隊多套系統 | **是** | 是 | 否 | 否 | 否 | 是 |
| 開源 | 否 | 否 | 否 | 否 | 否 | **是（MIT）** |
| 可在你的 IDE 內執行 | 否 | 否 | 否 | 否 | 否 | **是** |
| 底層模型 | Opus 4.7 | GPT 系 | Claude/GPT | GPT + Claude | Gemini | 自帶（BYO） |
| 定價 | Pro/Max/Team/Ent. | Figma Pro 加購 | 免費增值 | 免費增值 | 免費 beta | 免費 |

發布週的共識：**Claude Design** 在設計系統一致性、網頁擷取、協作上勝出。**Lovable** 在全端出貨上勝出。**Figma Make** 對 Figma 團隊最安全。**Stitch** 在純 token 生成上最強。**SuperDesign** 是唯一在 IDE 內執行的開源選項。

### 更多發布週比較

- [TechCrunch — Anthropic 推出 Claude Design](https://techcrunch.com/2026/04/17/anthropic-launches-claude-design-a-new-product-for-creating-quick-visuals/) — 主流媒體的發布定位：「快速視覺」工具，而非 Figma 殺手
- [Adweek — Claude Design 用於行銷素材、簡報與 UI](https://www.adweek.com/media/anthropic-debuts-claude-design-for-building-marketing-assets-decks-and-uis/) — 廣告代理視角，以行銷為先的解讀
- [PYMNTS — Anthropic 的設計工具叫板 Adobe 與 Figma](https://www.pymnts.com/artificial-intelligence-2/2026/anthropics-new-design-tool-rivals-adobe-and-figma/) — 對既有工具鏈的競爭定位
- [Trending Topics — Anthropic 挑戰 Lovable 與 Figma](https://www.trendingtopics.eu/anthropic-launches-claude-design-challenging-lovable-and-figma/) — 歐盟報導；認為 Lovable 才是更貼身的對手
- [Storyboard18 — Claude Design 震動設計軟體巨頭](https://www.storyboard18.com/digital/what-is-claude-design-anthropics-new-ai-tool-rattles-design-software-giants-ws-l-95581.htm) — 印度市場對 Figma/Adobe 漣漪效應的解讀
- [Web And IT News — 打在 Figma 的痛點上](https://www.webanditnews.com/2026/04/20/claude-design-hits-figma-where-it-hurts-ai-eats-into-non-designer-users/) — 主張切入點是非設計師，而非設計師
- [DEV（whoffagents）— CD vs Figma：到底改變了什麼](https://dev.to/whoffagents/claude-design-tool-vs-figma-what-actually-changed-and-when-to-use-each-3gj) — 實務工作者的並列比較與取捨
- [MindStudio — Claude Design vs Figma](https://www.mindstudio.ai/blog/claude-design-vs-figma) — 來自 AI 工具廠商視角的功能對照
- [Magic Patterns — Claude Design vs Figma Make](https://www.magicpatterns.com/blog/claude-design-vs-figma-make) — 聚焦提示詞到原型介面的窄向對決
- [eigent.ai — Claude Design vs Lovable，完整 2026 比較](https://www.eigent.ai/blog/claude-design-vs-lovable) — 設計工具與全端建構器在定價＋輸出品質上的差異
- [NxCode — 2026 氛圍設計工具：Stitch vs v0 vs Lovable vs Bolt](https://www.nxcode.io/resources/news/vibe-design-tools-compared-stitch-v0-lovable-2026) — 把 Claude Design 放進更大的氛圍設計版圖
- [Lushbinary — Claude Design vs Figma vs Canva vs Stitch](https://lushbinary.com/blog/claude-design-vs-figma-canva-google-stitch-comparison/) — 含 Canva（匯出目標）的四方矩陣

## 作品展示

用 Claude Design 實際做出來的成品 — 發布週初始種子有 10 張卡片（Tom's Guide 30 分鐘做出披薩品牌、Peter Yang 16 分鐘全部做完、Mercury 90% 推論、Brilliant 20→2 個提示詞、Datadog 一週→一場對話完成，等等）。

詳見 [`showcase/README.md`](showcase/README.md)。歡迎透過 [作品展示投稿 issue 範本](.github/ISSUE_TEMPLATE/showcase-submission.yml) 或 PR 投稿。

## 社群觀點

### 看好

> 「現在當 Figma 應該很難受。」
> — [r/ClaudeAI 發布討論串](https://www.reddit.com/r/ClaudeAI/comments/1so3k1y/)

> 「當了 29 年設計師，這是唯一更好的工作方式。」
> — [AI for Work](https://www.youtube.com/watch?v=4q2F4zblOLQ)

> 「設計系統整合在 AI 工具裡感覺是同類最佳。」
> — [@petergyang](https://x.com/petergyang/status/2045527271650558383)

- [Mejba Ahmed — Claude Code 缺的那層視覺](https://www.mejba.me/blog/claude-design-visual-workflow-claude-code) — 工程師正面解讀：補上 Claude Code 循環中缺的視覺缺口

### 看衰

> 「剛測完。這只對沒跟真正 UX/UI 設計師合作過的人有炒作價值。又一個燒 token 的爛功能。」
> — [r/ClaudeAI](https://www.reddit.com/r/ClaudeAI/comments/1so3k1y/)

> 「Anthropic 在說『看這隻手，有看到硬幣嗎？』— 我打開手，硬幣不在。但它從來就不在。整個目的是讓你不去看另一隻手在拿走你的訂閱費。」
> — [Malewicz](https://www.youtube.com/watch?v=IkspcJdeP3U)

> 「Google Stitch、Microsoft Designer 或 Template Monster 有達到中階設計師的品質嗎？沒有。這個有嗎？」
> — Malewicz，同一支影片

> 「Stickley 不會把松木染色冒充橡木。『忠於材料』意味著介面應該揭露它是用什麼做的，而不是裝成手繪，明明是組裝出來的。」
> — [Sam Henri Gold](https://samhenri.gold/blog/20260418-claude-design/)，Tavus 設計師，用工藝美術運動（Arts-and-Crafts）框架剖析 Claude Design，並預測 CD↔Claude Code 之間會形成雙向回饋循環

> 「Anthropic 推出 Claude Design — 因為誰還需要設計師？」
> — [The Register](https://www.theregister.com/2026/04/17/anthropic_debuts_claude_design/)，發布日標題

> 「如果你的工作就是做 comps（視覺稿），那你的工作本來就要消失。設計從來就不是 comps。」
> — [Christopher Noessel](https://christophernoessel.medium.com/design-was-never-the-comps-what-i-learned-when-claude-design-dumped-a-dozen-screens-on-me-73893af464ae)，IxDA 作者，在 Claude Design 一口氣丟給他十幾張畫面之後

> 「它取代的那些設計師，不是你擔心被取代的那些設計師。」
> — [Malewicz — Claude Design 會取代設計師嗎？](https://michalmalewicz.medium.com/will-claude-design-replace-designers-f92623f3befe)，YouTube 拆解的長文版

- [Abhi Chatterjee — 設計師的初次導覽](https://www.designsystemscollective.com/claude-design-just-launched-a-designers-first-walkthrough-c79d7ce47b9b) — 一套設計系統＋一個原型就燒掉約 50% 的週額度；訓練有素的眼睛仍能挑出間距不一致
- [PCWorld — 我用了半小時 Claude Design，已經被鎖一週](https://www.pcworld.com/article/3117811/i-tried-claude-design-for-half-an-hour-im-already-locked-out-for-a-week.html) — 30 分鐘的工作就把週額度耗盡

### 市場

Figma（NYSE: FIG）發布日收跌 **−4.26%**。據 r/FigmaDesign，盤中低點約 **−7%**。Adobe 持平。

- [Victoria Okwuokenye — Claude Design 完整剖析](https://medium.com/design-bootcamp/claude-design-is-here-full-breakdown-a32767258fb9) — 逐功能解讀 Claude Design 在既有設計工具鏈中的定位
- [BSWEN — 夠用於專業網站嗎？](https://docs.bswen.com/blog/2026-04-18-claude-design-quality-professional/) — 輸出品質門檻測試；主張到「專業網站」的差距比輿論說的更小

### 細項提醒

> 「好玩，但很快就燒光用量。」
> — [@petergyang](https://x.com/petergyang/status/2045527271650558383)

Opus 4.7 早期在長任務上的幻覺回報：[r/ClaudeCode 討論串](https://www.reddit.com/r/ClaudeCode/comments/1so9uta/) — 「花了 120 美元 API 額度，天啊有夠爛。」

- [Ocasio Consulting — Claude Design 評測](https://ocasioconsulting.com/claude-design-review/) — 直接呼籲改成固定的設計席位費；「配給創意有違工具精神」

### 論壇脈動

來自 Hacker News 的工程師社群觀點 — 三串討論、三種角度。

- [HN #47806725 — 主要發布討論串](https://news.ycombinator.com/item?id=47806725) — UI 稱職，但還沒有讓人驚艷
- [HN #47818700 — 「對 Claude Design 的想法與感受」](https://news.ycombinator.com/item?id=47818700) — 一坐下就用掉 95% 週額度；「玩具而非工具」的批評
- [HN #47832366 — 「Figma 的麻煩因 Claude Design 而加劇」](https://news.ycombinator.com/item?id=47832366) — 葉節點輸出 vs 完整設計生命週期；Figma 的曝險疊加

## 功能地圖

| 能力 | 說明 |
|---|---|
| 品牌導入 | Claude 讀取程式碼庫＋設計檔案，首次執行時自動建立系統 |
| 網頁擷取 | 從你的網站抓取線上元素，讓原型貼近正式環境 |
| 檔案匯入 | DOCX、PPTX、XLSX、圖片、Figma `.fig`、倉庫 URL、文字 |
| 行內註解 | 像在 Figma 一樣對特定元素留言 |
| 調整旋鈕 | 間距、顏色、版面的即時滑桿 — 可套用到整份設計 |
| 設計系統涵蓋範圍 | 顏色、字體、元件、預覽卡、可用的 UI kit、可匯出的 `SKILL.md` |
| 協作 | 組織範圍分享 — 私密、唯讀、可編輯權限，搭配群組 Claude 聊天 |
| 匯出 | Canva、PDF、PPTX、獨立 HTML、可分享的內部 URL、儲存資料夾 |
| 交接程式碼 | 一道指令打包 → Claude Code（CSS 變數＋元件 stub） |
| 前沿功能 | 語音、影片、shader、3D、內建 AI 輸出 |
| 影片 | 引用 @petergyang：「做出來的影片很漂亮，比簡報更出色」 |

## 發布時間軸

| 日期 | 事件 | 來源 |
|---|---|---|
| 2026-04-10 | Canva 在洛杉磯 Canva Create 上宣布與 Anthropic 合作（Canva Foundation Design Model 夥伴關係） | [Canva newsroom](https://www.canva.com/newsroom/news/canva-claude-design/) · [Morningstar / BusinessWire](https://www.morningstar.com/news/business-wire/20260410843169/canva-announces-anthropic-collaboration-to-bring-ai-powered-design-to-millions) |
| 2026-04-14 | The Information 爆料 Opus 4.7 ＋設計工具 | [r/singularity +889](https://www.reddit.com/r/singularity/comments/1slh72j/) |
| 2026-04-14 | Mike Krieger（Anthropic CPO）退出 Figma 董事會 — 發布前訊號 | [Martin Alderson](https://martinalderson.com/posts/anthropic-figma-supplier-conflict/) |
| 2026-04-17 | Claude Design ＋ Opus 4.7 以研究預覽形式推出 | [anthropic.com](https://www.anthropic.com/news/claude-design-anthropic-labs) |
| 2026-04-17 | 官方發布推文 | [@claudeai](https://x.com/claudeai/status/2045156267690213649) |
| 2026-04-17 | r/ClaudeAI 發布討論串達 2,293 讚 | [Reddit](https://www.reddit.com/r/ClaudeAI/comments/1so3k1y/) |
| 2026-04-17 | Figma 收跌 −4.26%（第二串討論 1,763 讚） | [Reddit](https://www.reddit.com/r/ClaudeAI/comments/1so6z2t/) · [@brewmarkets](https://x.com/brewmarkets/status/2045175784554283228) |
| 2026-04-17 | r/FigmaDesign 回報盤中約 −7% | [Reddit](https://www.reddit.com/r/FigmaDesign/comments/1soc1ic/) |
| 2026-04-17 | 主流媒體浪潮 — TechCrunch、VentureBeat、Adweek 定調發布 | [TechCrunch](https://techcrunch.com/2026/04/17/anthropic-launches-claude-design-a-new-product-for-creating-quick-visuals/) · [VentureBeat](https://venturebeat.com/ai/anthropic-launches-claude-design-ai-design-tool/) · [Adweek](https://www.adweek.com/media/anthropic-debuts-claude-design-for-building-marketing-assets-decks-and-uis/) |
| 2026-04-17 | Austin Lau（Anthropic 成長行銷）— 第一手 Tweaks 面板 demo ＋ Claude Cowork 登陸頁重現 | [@helloitsaustin](https://x.com/helloitsaustin/status/2045176910569980318) |
| 2026-04-18 | 拆解浪潮：Isenberg、Malewicz、02ui、Ray Fernando、WorldofAI、Vivek Mishra、AI for Work | 見 [影片拆解](#影片拆解) |
| 2026-04-18 | @petergyang 16 分鐘建構：影片＋簡報＋網站＋app ＋設計系統 | [推文](https://x.com/petergyang/status/2045527271650558383) |
| 2026-04-18 | Sam Henri Gold 發表「Stickley 接合工藝」框架文 | [samhenri.gold](https://samhenri.gold/blog/20260418-claude-design/) |
| 2026-04-18 | Brilliant ＋ Datadog 案例研究出現在 Anthropic 發布文中 | [anthropic.com](https://www.anthropic.com/news/claude-design-anthropic-labs) |
| 2026-04-18 | MacStories 由 John Voorhees 實測 — Apple 媒體視角；「對元素留言涵蓋了 95% 所需」 | [macstories.net](https://www.macstories.net/stories/hands-on-with-anthropic-labs-claude-design-preview/) |
| 2026-04-19 | Ryan Mather 發表 7 點訣竅串（系統先行、用註解而非聊天、connectors） | [@Flomerboy](https://x.com/Flomerboy/status/2045162321589252458) |
| 2026-04-19 | ADPList 社群提出「用 Claude Design 當 10x 設計師」框架 — `/packages/ui` 子目錄小撇步 | [adplist.substack.com](https://adplist.substack.com/p/how-to-become-a-10x-designer-with) |
| 2026-04-20 | 後續報導 —「打在 Figma 痛點」／「震動設計巨頭」 | [Web And IT News](https://www.webanditnews.com/2026/04/20/claude-design-hits-figma-where-it-hurts-ai-eats-into-non-designer-users/) · [Storyboard18](https://www.storyboard18.com/digital/what-is-claude-design-anthropics-new-ai-tool-rattles-design-software-giants-ws-l-95581.htm) |
| 2026-04-21 | 定價爭議 — Pro 方案失去 Claude Code 存取權 | [Pasquale Pillitteri](https://pasqualepillitteri.it/en/news/591/ai-app-builders-comparison-2026) |
| 2026-04-21 | DESIGN.md 規格由 Google（Stitch / Google Labs）開源 | [blog.google](https://blog.google/technology/google-labs/) |
| 2026-04-22 | Anthropic 發布 Claude Design 訂閱用量＋定價文件 | [support.claude.com](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing) |
| 2026-04-22 | 發布後報導收斂 — Lenny 迷你集 ＋ Quasa.io 訣竅 ＋ Anthropic 定價文件 | [Lenny's Newsletter](https://www.lennysnewsletter.com/p/what-claude-design-is-actually-good) · [Quasa.io](https://quasa.io/media/claude-design-looks-great-but-it-devours-your-token-limits-here-s-how-to-use-it-smartly) · [support.claude.com](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing) |

## 額度與 Token 預算

額度燒太快是社群第二大抱怨（僅次於 AI 罐頭風指紋）。以下是計算方式＋配方，讓你不會因為一個提示詞就賠掉一整週。

- **與聊天分開的計量。** Claude Design 有自己的用量計量，與一般 Claude.ai 聊天分開 — 出自 [Anthropic 定價文件](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing)。
- **依使用者計算，非共用池。** 週額度是每個席位獨立 — 團隊無法共用一個池 — 出自 [Anthropic 定價文件](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing)。
- **一次性促銷額度。** 大約等於 20 個典型提示詞，於 **2026-07-17** 到期 — 出自 [Anthropic 定價文件](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing)。拿去做實驗，把週額度留給正式工作。
- **視覺 token 約為文字的 3 倍。** Opus 4.7 視覺定價被廣泛引用；每張截圖、`.fig` 或網頁擷取都會墊高帳單。
- **Pro 可能 2–3 個提示詞就耗盡。** [r/ClaudeAI 發布討論串](https://www.reddit.com/r/ClaudeAI/comments/1so3k1y/) 上多則回報，兩個提示詞吃掉 95% 週上限。
- **30 分鐘 → 被鎖一週。** [PCWorld](https://www.pcworld.com/article/3117811/i-tried-claude-design-for-half-an-hour-im-already-locked-out-for-a-week.html) 評測一次就燒光整週額度。
- **一套設計系統＋一個原型 = 50% 週額度。** 來自 [Abhi Chatterjee](https://www.designsystemscollective.com/claude-design-just-launched-a-designers-first-walkthrough-c79d7ce47b9b) 的設計師實地回報。
- **「配給創意有違工具精神。」** [Ocasio Consulting](https://ocasioconsulting.com/claude-design-review/) 直接呼籲改成固定設計席位費。
- **Max-5x 上的具體美元成本：登陸頁 $3 / 影片 $4 / 簡報 $7。** [CopyRocket AI](https://copyrocket.ai/i-tested-claude-design-on-my-real-brand) 在真實品牌上測試，4–5 個提示詞燒掉 90% 週額度。權威的 token 預算參考。
- **圖片生成「部分由 Canva 驅動」。** [Lalindra（Pen With Paper）](https://medium.com/pen-with-paper/claude-design-review-i-spent-a-day-with-it-heres-what-actually-happens-441922202ef2) 指出 Claude Design 的圖片生成是透過 Canva Design Engine 夥伴關係 — 這解釋了視覺匯出在額度上的部分動態。

建議順序：[`recipes/token-budget-claude-design.md`](recipes/token-budget-claude-design.md) — 一次搭好骨架、把參考畫面上限設在 4 張、改用行內註解迭代、用分支做變體、一次打包到 Claude Code。

完整定價參考：[Claude Design 訂閱用量與定價 — support.claude.com](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing)。

## 官方資源

- [發布 — anthropic.com/news/claude-design-anthropic-labs](https://www.anthropic.com/news/claude-design-anthropic-labs)
- [產品 — claude.ai/design](https://claude.ai/design)
- [Anthropic Labs](https://www.anthropic.com/labs)
- [Anthropic Prompt Library](https://docs.anthropic.com/en/resources/prompt-library/library) — 品牌建構器、網站精靈、文案打磨器，另有 40+
- [`anthropics/skills` — `frontend-design` SKILL.md](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md) — Claude Design 底層所走的技能；Claude Code 處理 UI 工作時自動載入
- [`anthropics/skills` PR #210](https://github.com/anthropics/skills/pull/210) — 清晰度修訂；跨模型等級 75% 勝率，Haiku 提升最大
- [`anthropics/claude-cookbooks` — 前端美學 notebook](https://github.com/anthropics/claude-cookbooks/blob/main/coding/prompting_for_frontend_aesthetics.ipynb) — Anthropic 自家的反罐頭風入門；在 [反罐頭風工具包](#反罐頭風工具包) 中被引用
- [Claude Cookbooks — prompting_for_frontend_aesthetics.ipynb](https://github.com/anthropics/claude-cookbooks/blob/main/coding/prompting_for_frontend_aesthetics.ipynb)
- [提示詞工程總覽](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)
- [提示詞產生器（Console）](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/prompt-generator)

## X 訊號

發布週反應，附上出處。

| 帳號 | 角度 | 引言 | 連結 |
|---|---|---|---|
| [@claudeai](https://x.com/claudeai/status/2045156267690213649) | 官方 | 「介紹由 Anthropic Labs 推出的 Claude Design。由我們最強的視覺模型 Claude Opus 4.7 驅動。」 | 推文 |
| [@petergyang](https://x.com/petergyang/status/2045527271650558383) | 實作派 PM | 「設計系統整合在 AI 工具裡感覺是同類最佳。做出的影片很漂亮，比簡報更出色。好玩，但很快燒光用量。」 | 推文 |
| [@brewmarkets](https://x.com/brewmarkets/status/2045175784554283228) | 市場 | 「Anthropic 推出 Claude Design 後，Figma 股價正在重挫。」 | 推文 |

歡迎投稿更多：帳號、逐字引言（≤280 字元）、推文 URL、互動數字。

<p align="center"><img src="assets/mascot.svg" width="72" alt="mascot"></p>

## 各美學家族的 DESIGN.md

不依產業分類，而是依 **視覺性格** 分類 — 因為設計師實際上就是這樣挑的。每個家族連到 (1) `/design-md/<family>/` 中可用的 `DESIGN.md`、(2) 權威的外部參考、(3) 一行色票＋字體規格，讓你在抄之前就能目測合不合適。

**本倉庫已收錄的範例：** [warm/claude.md](design-md/warm/claude.md) · [warm/mercury.md](design-md/warm/mercury.md) · [warm/slima.md](design-md/warm/slima.md) · [terminal/ollama.md](design-md/terminal/ollama.md) · [terminal/warp.md](design-md/terminal/warp.md) · [terminal/opencode.md](design-md/terminal/opencode.md) · [editorial/linear.md](design-md/editorial/linear.md) · [editorial/vercel.md](design-md/editorial/vercel.md) · [data-dense/clickhouse.md](design-md/data-dense/clickhouse.md) · [data-dense/posthog.md](design-md/data-dense/posthog.md) · [data-dense/datadog.md](design-md/data-dense/datadog.md) · [data-dense/mongodb.md](design-md/data-dense/mongodb.md) · [data-dense/finlab.md](design-md/data-dense/finlab.md) · [data-dense/crewai.md](design-md/data-dense/crewai.md) · [data-dense/langfuse.md](design-md/data-dense/langfuse.md) · [cinematic/runway.md](design-md/cinematic/runway.md) · [cinematic/tavus.md](design-md/cinematic/tavus.md) · [cinematic/cohere.md](design-md/cinematic/cohere.md) · [cinematic/nvidia.md](design-md/cinematic/nvidia.md) · [cinematic/minimax.md](design-md/cinematic/minimax.md) · [cinematic/bmw.md](design-md/cinematic/bmw.md) · [cinematic/ferrari.md](design-md/cinematic/ferrari.md) · [cinematic/lamborghini.md](design-md/cinematic/lamborghini.md) · [cinematic/renault.md](design-md/cinematic/renault.md) · [playful/figma.md](design-md/playful/figma.md) · [playful/canva.md](design-md/playful/canva.md) · [playful/toss.md](design-md/playful/toss.md) · [playful/grab.md](design-md/playful/grab.md) · [glass/arc.md](design-md/glass/arc.md) · [glass/apple.md](design-md/glass/apple.md) · [brutalist/the-verge.md](design-md/brutalist/the-verge.md) · [indie/granola.md](design-md/indie/granola.md) · [remix/linear-x-claude.md](design-md/remix/linear-x-claude.md) · [remix/warp-x-sentry.md](design-md/remix/warp-x-sentry.md) · [remix/stripe-x-a24.md](design-md/remix/stripe-x-a24.md) · [remix/vercel-x-pitchfork.md](design-md/remix/vercel-x-pitchfork.md) · [remix/granola-x-criterion.md](design-md/remix/granola-x-criterion.md) · [remix/ollama-x-elevenlabs.md](design-md/remix/ollama-x-elevenlabs.md) · [remix/notion-x-duolingo.md](design-md/remix/notion-x-duolingo.md) · [remix/mercury-x-linear.md](design-md/remix/mercury-x-linear.md)

### 1. 編輯極簡（Editorial Minimalism）

冷靜的中性色、襯線或窄無襯線標題、寬鬆行高、單一強調色。為閱讀、定價頁、文件而生。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| Linear | `#fff / #0f0f14 / #5e6ad2` | Inter / Söhne | [linear.app](https://linear.app) |
| Stripe | `#fff / #0a2540 / #635bff` | Sohne / Camphor | [stripe.com](https://stripe.com) |
| Vercel | `#fff / #000 / 單一灰階梯度` | Geist | [vercel.com](https://vercel.com) |
| Mintlify | `#fff / #0c0c0e / 綠色強調` | Inter 閱讀最佳化 | [mintlify.com](https://mintlify.com) |

### 2. 終端機核心（Terminal-Core）

到處都是等寬字、近黑底上的磷光綠或琥珀色、硬邊、CLI 隱喻。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| Ollama | `#000 / #fff / 無強調色` | 等寬 | [ollama.com](https://ollama.com) |
| Warp | `#0b0d14 / #16d5e6 / #ff7a59` | Roobert + JetBrains Mono | [warp.dev](https://warp.dev) |
| Raycast | `#1d1d1f / #ff6363 / 白` | 自訂 sans + 等寬 | [raycast.com](https://raycast.com) |
| OpenCode | `#080808 / #d2d2d2 / 綠` | IBM Plex Mono | [opencode.ai](https://opencode.ai) |

### 3. 暖色編輯（Warm Editorial）

陶土色、奶油色、黏土色。襯線內文、親切、有人味。Claude 自家品牌就屬於這裡。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| Claude / Anthropic | `#f4f3ee / #c96442 / #191817` | Styrene / Tiempos | [anthropic.com](https://anthropic.com) |
| Notion | `#fff / #37352f / 暖灰` | Segoe + Lyon serif | [notion.so](https://notion.so) |
| Resend | `#0a0a0a / #fff / 等寬強調` | Söhne + GT America Mono | [resend.com](https://resend.com) |
| Substack | `#fff / #1a1a1a / #ff6719` | Spectral + SF Pro | [substack.com](https://substack.com) |
| Slima | `#faf9f6 / #f3f1ec 暖紙 / #0a0a0a / 琥珀+綠+靛（功能性）` | IBM Plex Serif + Inter | [slima.ai](https://slima.ai/zh-TW) |

### 4. 資料密集專業（Data-Dense Pro）

圖表是主角。緊湊間距、飽和的分類色盤、固定寬度數字、暗色優先的儀表板。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| ClickHouse | `#181818 / #faff69 / magenta` | Inter tabular | [clickhouse.com](https://clickhouse.com) |
| PostHog | `#1d4aff / #f9bd2b / #000` | Matter + Mono | [posthog.com](https://posthog.com) |
| Grafana | `#111217 / #f47c1b / 多序列` | Inter | [grafana.com](https://grafana.com) |
| Sentry | `#362d59 / #f6827d / #584774` | Rubik | [sentry.io](https://sentry.io) |
| Supabase | `#171717 / #3ecf8e` | 自訂 + 等寬 | [supabase.com](https://supabase.com) |
| MongoDB | `#001e2b / #00ed64 / #00684a` | Euclid Circular A + Source Code Pro | [mongodb.com](https://mongodb.com) |
| FinLab | `#ffffff / #2563eb / #16a34a 漲 / #dc2626 跌` | Inter tabular + CJK 字組 | [finlab.finance](https://finlab.finance) |
| CrewAI | `#0b0e14 / #ff5e4d / #2dd4a7 成功 / #f0506a 失敗` | Inter tabular + JetBrains Mono | [crewai.com](https://crewai.com) |
| Langfuse | `#f6f5ef / #0a0a0a / #f5f56b 螢光標記` | Inter tabular + JetBrains Mono | [langfuse.com](https://langfuse.com) |

### 5. 電影感暗色（Cinematic Dark）

電影級漸層、超大字、動態優先、媒體量大的主視覺。為 AI 產品與創作者工具而生。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| RunwayML | `#000 / 飽和洋紅 + 青` | 自訂 grotesque | [runwayml.com](https://runwayml.com) |
| ElevenLabs | `#0a0a0a / 電光藍 / 波形母題` | Inter | [elevenlabs.io](https://elevenlabs.io) |
| Minimax | `#000 / 炭灰上的霓虹萊姆綠` | 自訂 + 等寬 | [minimax.ai](https://minimax.ai) |
| Midjourney | `#000 / 大地色 + 淡紫` | 編輯襯線 | [midjourney.com](https://midjourney.com) |
| NVIDIA | `#000 / #76b900 招牌綠 / #ffffff` | NVIDIA Sans / Helvetica Neue | [nvidia.com](https://nvidia.com) |
| BMW | `#fff / #1c69d4 企業藍 / M 漸層` | BMW Type Next Web + Helvetica Neue | [bmw.com](https://bmw.com) |
| Ferrari | `#000 / #fff / #eb2323 Rosso Corsa` | FerrariSans | [ferrari.com](https://ferrari.com) |
| Lamborghini | `#000 / #ffc000 暖金 / 六角母題` | LamboType + Roboto | [lamborghini.com](https://lamborghini.com) |
| Renault | `#fff / 極光黃→洋紅→青 / #efdf00 + #e91630` | NouvelR | [renault.fr](https://renault.fr) |

### 6. 趣味色彩（Playful Color）

高飽和、插畫式強調、圓角、裝飾性形狀。親近消費者。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| Figma | `#0acf83 / #f24e1e / #a259ff / #ff7262 / #1abcfe` | Inter + Whyte | [figma.com](https://figma.com) |
| Clay | `#f6e9c9 / 有機形狀 / 柔和漸層` | Söhne | [clay.com](https://clay.com) |
| Duolingo | `#58cc02 / #fff / #ff4b4b` | DIN Rounded | [duolingo.com](https://duolingo.com) |
| Mailchimp | `#ffe01b / #000` | Cooper Hewitt + GT America | [mailchimp.com](https://mailchimp.com) |
| Cal.com | `#292929 / #fff / 單一強調色` | Inter | [cal.com](https://cal.com) |
| Toss | `#fff / #3182f6 Toss 藍 / #191f28` | Toss Product Sans + Noto Sans KR | [toss.im](https://toss.im) |
| Grab | `#fff / #00b14f Grab 綠 / #00692e / #1a1a1a` | 圓體 sans（Poppins/Inter）+ 東南亞文字 | [grab.com](https://www.grab.com/sg/) |

### 7. 玻璃／柔未來感（Glass / Soft-Futurism）

霧面模糊、層疊半透明、柔和漸層、貼近 Apple。高級消費感。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| Apple | `#fff / #1d1d1f / 系統色` | SF Pro | [apple.com](https://apple.com) |
| Arc Browser | `#fff / 放射狀粉彩漸層` | 自訂 | [arc.net](https://arc.net) |
| Airbnb | `#fff / #ff385c / #222` | Cereal | [airbnb.com](https://airbnb.com) |
| Granola | `#faf8f2 / 暖色玻璃` | 編輯襯線 | [granola.ai](https://granola.ai) |
| Spotify | `#000 / #1db954` | Circular | [spotify.com](https://spotify.com) |

### 8. 霓虹粗獷（Neon Brutalist）

硬邊、刻意「醜」的字體混搭、超大數字、飽和單色。宣言型作品。

| 品牌 | 色票 | 字體 | 外部參考 |
|---|---|---|---|
| Bugatti | `#0d1321 / 電光藍 / 鉻` | 自訂 + GT America | [bugatti.com](https://bugatti.com) |
| PlayStation | `#000 / 全光譜稜鏡` | SST | [playstation.com](https://playstation.com) |
| The Verge | `#ff6600 / #000 / #fff` | Polysans + 編輯襯線 | [theverge.com](https://theverge.com) |
| Pitchfork | `#fff / #000 / #ff5d1f` | 編輯襯線 | [pitchfork.com](https://pitchfork.com) |

### 9. 小眾／獨立精選（非財星 500 大）

VoltAgent 目錄沒收錄的品牌 — 獨立 SaaS、小眾工具、雜誌、博物館、遊戲工作室。維護者的偏好：這些才是值得抄的。

| 品牌 | 為什麼 | 外部參考 |
|---|---|---|
| Thesephist / Ink & Switch | 研究出版品美學 | [thesephist.com](https://thesephist.com) |
| Paradigm | 加密公司的極簡襯線 | [paradigm.xyz](https://paradigm.xyz) |
| Criterion Collection | 電影檔案編輯風 | [criterion.com](https://criterion.com) |
| A24 | 把電影品牌當作藝術品 | [a24films.com](https://a24films.com) |
| Letterboxd | 暗色影迷社群 | [letterboxd.com](https://letterboxd.com) |
| ProPublica | 調查報導的資訊密度 | [propublica.org](https://propublica.org) |
| Dimension.dev | 開發者工具的柔漸層 | [dimension.dev](https://dimension.dev) |
| Granola | AI 筆記工具的暖意 | [granola.ai](https://granola.ai) |
| Superhuman | 高級電子郵件極簡 | [superhuman.com](https://superhuman.com) |
| Obsidian | 個人知識庫暗色 | [obsidian.md](https://obsidian.md) |

### 外部目錄

DESIGN.md 生態系比本倉庫大得多。我們只收錄別人沒收的 — 以下是值得加書籤的上游、鏡像、姊妹清單與原始規格來源。

**DESIGN.md 生態系**

- [**VoltAgent/awesome-claude-design**](https://github.com/VoltAgent/awesome-claude-design) <img src="https://img.shields.io/github/stars/VoltAgent/awesome-claude-design?style=flat-square&logo=github&label=" height="16"> — 68 個品牌 DESIGN.md 檔案，依產業分類（權威的產業目錄）
- [**VoltAgent/awesome-design-md**](https://github.com/VoltAgent/awesome-design-md) <img src="https://img.shields.io/github/stars/VoltAgent/awesome-design-md?style=flat-square&logo=github&label=" height="16"> — 59+ 品牌的 Stitch 格式，每筆都附 preview.html（與工具無關的雙生版）
- [**philquist/awesome-claude-design-examples**](https://github.com/philquist/awesome-claude-design-examples) <img src="https://img.shields.io/github/stars/philquist/awesome-claude-design-examples?style=flat-square&logo=github&label=" height="16"> — VoltAgent 收藏的社群鏡像／分叉，可作探索入口
- [**getdesign.md**](https://getdesign.md/) — 可瀏覽的網頁 UI，收 60+ DESIGN.md（Cursor、Vercel、Warp、Claude、Mistral、xAI、Tesla、Renault、Revolut、Wise、Linear、PostHog）
- [**google-labs-code/design.md**](https://github.com/google-labs-code/design.md) <img src="https://img.shields.io/github/stars/google-labs-code/design.md?style=flat-square&logo=github&label=" height="16"> — Google Labs Code 官方 DESIGN.md 規格，Apache 2.0；見 [`docs/spec.md`](https://github.com/google-labs-code/design.md/blob/main/docs/spec.md)

**主題彙整**

- [**github.com/topics/design-md**](https://github.com/topics/design-md) — 此格式本身的自動滾動倉庫流
- [**github.com/topics/claude-design**](https://github.com/topics/claude-design) — 帶 Claude Design 標籤的倉庫（技能、範例、工具）

**Awesome-Claude 元清單**

- [**rohitg00/awesome-claude-code-toolkit**](https://github.com/rohitg00/awesome-claude-code-toolkit) <img src="https://img.shields.io/github/stars/rohitg00/awesome-claude-code-toolkit?style=flat-square&logo=github&label=" height="16"> — 姊妹元工具包：135 個 agents、35 個 skills、42 個 commands、176 個 plugins
- [**hesreallyhim/awesome-claude-code**](https://github.com/hesreallyhim/awesome-claude-code) <img src="https://img.shields.io/github/stars/hesreallyhim/awesome-claude-code?style=flat-square&logo=github&label=" height="16"> — 最初的 awesome-claude-code 清單；收錄 Patrick Ellis 的 Design Review Workflow
- [**jqueryscript/awesome-claude-code**](https://github.com/jqueryscript/awesome-claude-code) <img src="https://img.shields.io/github/stars/jqueryscript/awesome-claude-code?style=flat-square&logo=github&label=" height="16"> — 帶出 claude-design-engineer（1.1k 星）與 excalidraw-diagram-skill（1.2k 星）
- [**sickn33/antigravity-awesome-skills**](https://github.com/sickn33/antigravity-awesome-skills) <img src="https://img.shields.io/github/stars/sickn33/antigravity-awesome-skills?style=flat-square&logo=github&label=" height="16"> — 1,431+ 技能，含 Leonxlnx/taste-skill（Stitch 設計系統、粗獷／極簡模式）
- [**ComposioHQ/awesome-claude-skills**](https://github.com/ComposioHQ/awesome-claude-skills) <img src="https://img.shields.io/github/stars/ComposioHQ/awesome-claude-skills?style=flat-square&logo=github&label=" height="16"> — 強調 claude.ai + Code + API 可攜性；附 canvas-design SKILL.md
- [**BehiSecc/awesome-claude-skills**](https://github.com/BehiSecc/awesome-claude-skills) <img src="https://img.shields.io/github/stars/BehiSecc/awesome-claude-skills?style=flat-square&logo=github&label=" height="16"> — 偏安全性的技能清單，與設計工程交叉
- [**travisvn/awesome-claude-skills**](https://github.com/travisvn/awesome-claude-skills) <img src="https://img.shields.io/github/stars/travisvn/awesome-claude-skills?style=flat-square&logo=github&label=" height="16"> — 精選技能，含子代理指引與撰寫慣例
- [**heilcheng/awesome-agent-skills**](https://github.com/heilcheng/awesome-agent-skills) <img src="https://img.shields.io/github/stars/heilcheng/awesome-agent-skills?style=flat-square&logo=github&label=" height="16"> — 多代理（Claude/Cursor/Codex/Gemini）技能，明確交叉連結 awesome-design-md
- [**quemsah/awesome-claude-plugins**](https://github.com/quemsah/awesome-claude-plugins) <img src="https://img.shields.io/github/stars/quemsah/awesome-claude-plugins?style=flat-square&logo=github&label=" height="16"> — 設計工程外掛，帶工藝／記憶／強制執行框架
- [**awesomeclaude.ai**](https://awesomeclaude.ai) — 跨 awesome-claude-* 倉庫的網頁目錄，含 awesome-claude-agents 子區

**工具與擷取器**

- [**yuvrajangadsingh/brandmd**](https://github.com/yuvrajangadsingh/brandmd) <img src="https://img.shields.io/github/stars/yuvrajangadsingh/brandmd?style=flat-square&logo=github&label=" height="16"> — `npx brandmd https://linear.app` 產生 DESIGN.md / CSS 自訂屬性 / Tailwind v4 / 暗色模式覆寫；無 LLM 呼叫；以 Agent Skill 形式在 30+ 平台發布
- [**bitjaru/styleseed**](https://github.com/bitjaru/styleseed) <img src="https://img.shields.io/github/stars/bitjaru/styleseed?style=flat-square&logo=github&label=" height="16"> — 69 條設計規則 + 48 個 shadcn 元件 + Toss/Stripe/Linear/Vercel/Notion 品牌皮膚；教 LLM 設計師如何思考，而不只是品牌長相
- [**Muluk-m/design-distill**](https://github.com/Muluk-m/design-distill) <img src="https://img.shields.io/github/stars/Muluk-m/design-distill?style=flat-square&logo=github&label=" height="16"> — Stitch 相容的 DESIGN.md 產生器，預先打包 github / linear / notion / stripe / vercel 快照；可搭配 Codex、Claude Code 與任何 AI 客戶端
- [**bergside/design-md-chrome**](https://github.com/bergside/design-md-chrome) <img src="https://img.shields.io/github/stars/bergside/design-md-chrome?style=flat-square&logo=github&label=" height="16"> — Chrome / Firefox / Edge 擴充功能，以 TypeUI 格式從任何網站擷取 DESIGN.md + SKILL.md（[Chrome 線上應用程式商店](https://chromewebstore.google.com/detail/designmd-style-extractor/ogpdnchdjiibhobphelbbkemnnemkfma)）；對設計師友善、不需終端機

**背景閱讀**

- [**OSS Insight — DESIGN.md Protocol 2026**](https://ossinsight.io/blog/design-md-protocol-2026) — awesome-design-md 爆紅的歷史時間軸；有助理解此格式如何擴散
- [**Google Stitch 開源公告**](https://medium.com/design-bootcamp/google-makes-design-md-open-source-on-its-way-to-become-a-industry-standard-16119f2368dd) — fernandocomet 對 Google 開源 DESIGN.md 規格的報導
- [**MindStudio — 什麼是 Design.md**](https://www.mindstudio.ai/blog/what-is-design-md) — 給非設計師／工具採購者的格式入門

<p align="center"><img src="assets/divider.svg" width="600" alt="divider"></p>

## 混搭配方 Remix

單一品牌的複製很快就變得平庸。把不同家族的 tokens 混在一起，做出新鮮的樣貌。

| 名稱 | 配方 | 感覺 |
|---|---|---|
| **Linear × Claude** | Linear 的字體 + Claude 的陶土強調色 + 暖中性 | 有靈魂的編輯型 SaaS |
| **Warp × Sentry** | Warp 的等寬網格 + Sentry 的淡紫→紫 | 不冰冷的開發者工具儀表板 |
| **Stripe × A24** | Stripe 的版面紀律 + A24 的海報大膽 | 有個性的金融科技簡報 |
| **Vercel × Pitchfork** | Vercel 的灰階梯度 + Pitchfork 的橘 | 編輯型文件站 |
| **Granola × Criterion** | Granola 的暖意 + Criterion 的編輯嚴謹 | 有份量的高級筆記 app |
| **Ollama × ElevenLabs** | 終端機等寬 + 電影感暗色漸層 | CLI 工具登陸頁 |
| **Notion × Duolingo** | Notion 的中性 + Duolingo 的綠 | 親切的教育 SaaS |
| **Mercury × Linear** | Mercury 的奶油 + 靛藍 + Linear 的精準密度 | 帶編輯暖意的金融科技儀表板 |

出貨你的混搭：`/design-md/remix/<name>.md` + 截圖。發 PR。

## 如何選擇家族

三個問題，挑一個家族。

1. **你的產品偏重閱讀還是偏重掃視？**
   - 偏閱讀 → [編輯極簡](#各美學家族的-designmd) 或 [暖色編輯](#各美學家族的-designmd)
   - 偏掃視 → [資料密集專業](#各美學家族的-designmd) 或 [終端機核心](#各美學家族的-designmd)

2. **使用者是誰？**
   - 開發者 → [終端機核心](#各美學家族的-designmd) 或 [資料密集專業](#各美學家族的-designmd)
   - 設計師／創作者 → [電影感暗色](#各美學家族的-designmd) 或 [趣味色彩](#各美學家族的-designmd)
   - 一般消費者 → [玻璃／柔未來感](#各美學家族的-designmd) 或 [趣味色彩](#各美學家族的-designmd)
   - 專業消費者（prosumer） → [暖色編輯](#各美學家族的-designmd)

3. **品牌需要看起來「有膽量」嗎？**
   - 需要 → [霓虹粗獷](#各美學家族的-designmd) 或 [小眾／獨立精選](#各美學家族的-designmd)
   - 不需要 → 留在第 1–7 家族

## 提示詞與食譜

### 官方（Anthropic）

- [Anthropic Prompt Library](https://docs.anthropic.com/en/resources/prompt-library/library) — 40+ 提示詞，含 **品牌建構器**、**網站精靈**、**文案打磨器**
- [claude-cookbooks / prompting_for_frontend_aesthetics.ipynb](https://github.com/anthropics/claude-cookbooks/blob/main/coding/prompting_for_frontend_aesthetics.ipynb) — 官方反罐頭風 notebook
- [系統提示詞發行說明](https://docs.anthropic.com/en/release-notes/system-prompts)

### 社群 gist 與提示詞倉庫

- [**superdesigndev/superdesign**](https://github.com/superdesigndev/superdesign) <img src="https://img.shields.io/github/stars/superdesigndev/superdesign?style=flat-square&logo=github&label=" height="16"> — 由 [@jasonzhou1993](https://x.com/jasonzhou1993) 與 [@jackjack_eth](https://x.com/jackjack_eth) 打造、在 IDE 內的開源設計代理。平行 Claude Code 代理、無限畫布 UX。[Show HN](https://news.ycombinator.com/item?id=44376003)
- [**jonthebeef/superdesign-mcp-claude-code**](https://github.com/jonthebeef/superdesign-mcp-claude-code) <img src="https://img.shields.io/github/stars/jonthebeef/superdesign-mcp-claude-code?style=flat-square&logo=github&label=" height="16"> — 把 SuperDesign 接進 Claude Code 的 MCP 伺服器，免 API key
- [**Owl-Listener/designer-skills**](https://github.com/Owl-Listener/designer-skills) <img src="https://img.shields.io/github/stars/Owl-Listener/designer-skills?style=flat-square&logo=github&label=" height="16"> — MC Dean 的 Designer Skills Collection。MIT
- [**Owl-Listener/designpowers**](https://github.com/Owl-Listener/designpowers) <img src="https://img.shields.io/github/stars/Owl-Listener/designpowers?style=flat-square&logo=github&label=" height="16"> — 專家設計代理，Direct + Auto 模式。MIT
- [**saifyxpro/ui-ux-design-pro-skill**](https://github.com/saifyxpro/ui-ux-design-pro-skill) <img src="https://img.shields.io/github/stars/saifyxpro/ui-ux-design-pro-skill?style=flat-square&logo=github&label=" height="16"> — 風格、色盤、字體、推理規則、平台範本
- [**nextlevelbuilder/ui-ux-pro-max-skill**](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) <img src="https://img.shields.io/github/stars/nextlevelbuilder/ui-ux-pro-max-skill?style=flat-square&logo=github&label=" height="16"> — 跨平台的專業 UI/UX
- [**alirezarezvani/claude-skills**](https://github.com/alirezarezvani/claude-skills) <img src="https://img.shields.io/github/stars/alirezarezvani/claude-skills?style=flat-square&logo=github&label=" height="16"> — 橫跨工程、行銷、產品、合規的技能
- [**NicholasSpisak — Design with Claude Code**](https://gist.github.com/NicholasSpisak/7cb9db221b0b7c4c4aaf9ffca21a847c) — `design.md` 提示詞，三位設計專家人格即時辯論
- [**abhishekray07/claude-md-templates**](https://github.com/abhishekray07/claude-md-templates) <img src="https://img.shields.io/github/stars/abhishekray07/claude-md-templates?style=flat-square&logo=github&label=" height="16"> — CLAUDE.md + `api-design.md` 規則範本
- [**smartwhale8/claude-playbook**](https://github.com/smartwhale8/claude-playbook) <img src="https://img.shields.io/github/stars/smartwhale8/claude-playbook?style=flat-square&logo=github&label=" height="16"> — 正式環境 `.claude/` 鷹架，GitHub 範本
- [**VoltAgent/awesome-agent-skills**](https://github.com/VoltAgent/awesome-agent-skills) — 1000+ 技能，含 `design-md`、`enhance-prompt`、`react-components`、`shadcn-ui`
- [**daymade/claude-code-skills**](https://github.com/daymade/claude-code-skills) — 可上線的 Claude Code 技能市集

### 本倉庫附的提示詞包（`/prompts`）

每個包都含完整提示詞、附預期輸出的範例執行、品質檢查與變體。

| 包 | 用途 | 檔案 |
|---|---|---|
| `brand-to-design-md` | URL → 含 9 個標準章節的完整 DESIGN.md | [`/prompts/brand-to-design-md.md`](prompts/brand-to-design-md.md) |
| `audit-live-site` | URL → 評分稽核（層級、間距、無障礙、AI 罐頭風）＋ 待辦清單 | [`/prompts/audit-live-site.md`](prompts/audit-live-site.md) |
| `3-designer-debate` | 三方批評，含綜合結論＋少數意見報告 | [`/prompts/3-designer-debate.md`](prompts/3-designer-debate.md) |
| `remix-two-brands` | 結合兩個 DESIGN.md，並明確仲裁 token 衝突 | [`/prompts/remix-two-brands.md`](prompts/remix-two-brands.md) |
| `family-picker` | 3 個問題 → 推薦家族 ＋ 2 個參考 DESIGN.md | [`/prompts/family-picker.md`](prompts/family-picker.md) |

索引：[`/prompts/README.md`](prompts/README.md)

## 反罐頭風工具包

把這段片段丟進 Claude Design 的系統提示詞，或任何 Claude Code 專案。出自 Anthropic 的 [前端美學 cookbook](https://github.com/anthropics/claude-cookbooks/blob/main/coding/prompting_for_frontend_aesthetics.ipynb)：

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

Malewicz 的 [拆解](https://www.youtube.com/watch?v=IkspcJdeP3U) <img src="https://img.shields.io/youtube/views/IkspcJdeP3U?style=flat-square&label=views&color=191817" height="16"> 開場就點名 Claude Design 自己的 logo「很通用、配色」— 正是這段提示詞要避開的陷阱。

### Claude Design 的預設指紋（避開）

社群最大的單一抱怨：每個 Claude Design 輸出看起來都一樣。以下整理自發布週的 Reddit 討論串、[Sam Henri Gold 部落格文](https://samhenri.gold/blog/20260418-claude-design/)、[Banani 評測](https://www.banani.co/blog/claude-design-review)，以及 [The Neuron Daily 彙整](https://www.theneurondaily.com/p/anthropic-s-claude-design-launched-and-reddit-has-thoughts)。

| 指紋 | 長相 | 反制規則 |
|---|---|---|
| **到處都是藍綠強調色** | 預設接近 `#16d5e6` 的動作色出現在 CTA、標題強調、focus ring、圖表填色 | 在第一次生成前就在 DESIGN.md 指定品牌專屬強調色 |
| **閃爍的狀態點** | 導覽列右上角的綠／萊姆動畫點，反射性地表示「即時」／「AI」 | 在提示詞中拒絕：「不要動畫狀態指示器」 |
| **容器湯** | 一層層 pill 包卡片包卡片包內容；padding 疊 24/24/24 | 限制巢狀深度：「容器最多巢狀 2 層」 |
| **預設襯線標題** | 近似 Tiempos 或 Source Serif 的襯線配 sans 內文 — 像 Anthropic 品牌的剩菜 | 明確指定字組＋字重＋字距，而不是給一個氛圍 |
| **每張卡片左側的強調條** | 不分語意，每張卡片都有 4px 彩色直條 | 把左側直條保留給單一角色（例如嚴重度）— 絕不當裝飾 |
| **主視覺的三欄功能格** | 模型產出的登陸頁幾乎都是同一個 section-2 版面 | 簡報需求：「不要三欄功能格；改用跑馬燈、交錯列或單欄」 |
| **Lucide 圖示堆** | 導覽、按鈕、空狀態都用同一套預設圖示 | 要嘛固定單一圖示家族（Phosphor / Heroicons / 自訂），要嘛純文字 |
| **生成主視覺忽略產品色盤** | 圖片生成器挑「看起來對」的顏色，卻無視 DESIGN.md 的 tokens | 約束圖片：「只用 `--bg`、`--accent`、`--text` 重新生成主視覺」 |

用專屬提示詞包 [`prompts/break-default-aesthetic.md`](prompts/break-default-aesthetic.md)，一次貼上就能中和這些。

### 這些預設是怎麼來的

Claude Design 走的是 Anthropic 開源的 [`frontend-design` 技能](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md) — 與 Claude Code 處理 UI 工作時自動載入的是同一個。該技能的預設偏向「第一版就達正式品質」，在沒有 DESIGN.md 的情況下，每次都會落在同一個樣貌。

兩個值得加書籤的相關 Anthropic 資源：

- [**前端美學 cookbook**](https://github.com/anthropics/claude-cookbooks/blob/main/coding/prompting_for_frontend_aesthetics.ipynb) — Anthropic 自家的反罐頭風入門；上面引用的來源
- [**`skills` PR #210**](https://github.com/anthropics/skills/pull/210) — frontend-design 技能的清晰度修訂；跨模型等級 75% 勝率，Haiku 提升最大

Anthropic 在 cookbook 中承認了這個問題：*「你傾向收斂到通用、『分佈內』的輸出。在前端設計上，這造就了使用者所謂的『AI 罐頭風』美學。要避開它：做出有創意、有辨識度、會讓人驚喜的前端。」*

### 社群反罐頭風工具

除了 Anthropic 自家素材，社群也針對上面整理的罐頭指紋，做出越來越多技能、外掛與審查流程。可作為提示詞片段的替代或補充。

- [**Leonxlnx/taste-skill**](https://github.com/Leonxlnx/taste-skill) <img src="https://img.shields.io/github/stars/Leonxlnx/taste-skill?style=flat-square&logo=github&label=" height="16"> — 前端品味技能：高級 UI 生成、改版稽核、GSAP 動態、粗獷／極簡／柔和變體、三段旋鈕參數化（變異度、動態、密度）
- [**Dammyjay93/interface-design**](https://github.com/Dammyjay93/interface-design) <img src="https://img.shields.io/github/stars/Dammyjay93/interface-design?style=flat-square&logo=github&label=" height="16"> — 給 Claude Code 的設計工程（前身 `claude-design-engineer`）：持久設計系統檔案、init/audit/extract 斜線指令、跨工作階段強制 token 一致
- [**coleam00/excalidraw-diagram-skill**](https://github.com/coleam00/excalidraw-diagram-skill) <img src="https://img.shields.io/github/stars/coleam00/excalidraw-diagram-skill?style=flat-square&logo=github&label=" height="16"> — 用視覺論證、而非隨手拍方塊箭頭的圖表技能；Playwright 渲染—驗證循環抓出重疊、未對齊、間距不良
- [**OneRedOak/claude-code-workflows — design-review**](https://github.com/OneRedOak/claude-code-workflows/tree/main/design-review) <img src="https://img.shields.io/github/stars/OneRedOak/claude-code-workflows?style=flat-square&logo=github&label=" height="16"> — Patrick Ellis 的 UI/UX 審查流程：子代理 + `/design-review` 斜線指令 + CLAUDE.md 記憶整合 + 透過 Playwright MCP 涵蓋無障礙
- [**ComposioHQ/awesome-claude-skills — canvas-design**](https://github.com/ComposioHQ/awesome-claude-skills/blob/master/canvas-design/SKILL.md) <img src="https://img.shields.io/github/stars/ComposioHQ/awesome-claude-skills?style=flat-square&logo=github&label=" height="16"> — 用視覺表達設計哲學：兩階段（哲學 → 成品）、90% 視覺 / 10% 必要文字、結構上反範本
- [**Marie Claire Dean — 63 個設計技能**](https://marieclairedean.substack.com/p/i-built-63-design-skills-for-claude)（[倉庫](https://github.com/Owl-Listener/designer-skills) <img src="https://img.shields.io/github/stars/Owl-Listener/designer-skills?style=flat-square&logo=github&label=">）— 63 技能 + 27 指令，橫跨研究、系統、策略、UI、互動、原型、營運；教 Claude *設計到底是什麼*，而不只是生圖。MIT

### 外洩的系統提示詞

Claude Design 的 frontend-design 技能實際上寫了什麼，來自社群逆向工程。在調整你的 DESIGN.md 之前先讀這些 — 上面每條反制規則都對應回這份提示詞中的某個預設。

- [**GordenSun gist — 擷取出的 Claude Design 系統提示詞**](https://gist.github.com/GordenSun/b5c6316f078d694645ca466386875296) — 完整擷取的提示詞；把 Claude 定位為「以使用者為經理的專家設計師」，走 Frontend design 技能，並要模型「先理解視覺詞彙」。主要反罐頭風參考：解釋了 *為什麼* 輸出會預設成上面整理的藍綠美學指紋。
- [**hqman gist — 另一份系統提示詞擷取**](https://gist.github.com/hqman/f46d5479a5b663c282c94faa8be866de) — 第二份外洩擷取；可交叉比對工作階段／模型等級間的差異。有助辨別哪些指令是穩定預設、哪些是工作階段注入的變化。

## 技能與外掛

可與 Claude Design 搭配的 Claude Code 技能與 SkillKit 外掛。

- [**design-shotgun**](https://github.com/rohitg00/skillkit) — 生成 N 個變體，並列比較
- [**design-html**](https://github.com/rohitg00/skillkit) — 把定稿 mockup → 正式 HTML/CSS
- [**design-review**](https://github.com/rohitg00/skillkit) — 設計師之眼 QA、AI 罐頭風偵測
- [**design-consultation**](https://github.com/rohitg00/skillkit) — 完整系統提案（美學、字體、顏色、動態）
- [**plan-design-review**](https://github.com/rohitg00/skillkit) — 實作前在 plan 模式批評
- [**plan-devex-review**](https://github.com/rohitg00/skillkit) — 面向開發者 UI 的 DX 稽核
- [**google-labs-code/design-md**](https://github.com/VoltAgent/awesome-agent-skills) — 權威的 Stitch DESIGN.md 產生器
- [**superdesign-mcp**](https://github.com/jonthebeef/superdesign-mcp-claude-code) — 把 SuperDesign 當作 Claude Code MCP 伺服器

透過 SkillKit 安裝：`npx skillkit install design-shotgun`

### 社群安裝

上面列出的同一批反罐頭風工具，附明確安裝指令。可自由混搭 — 多數能與上面的 SkillKit 包乾淨串接。

- [**Leonxlnx/taste-skill**](https://github.com/Leonxlnx/taste-skill) <img src="https://img.shields.io/github/stars/Leonxlnx/taste-skill?style=flat-square&logo=github&label=" height="16"> — 高級 UI 生成、改版稽核、GSAP 動態、粗獷／極簡／柔和變體
  ```sh
  npx skills add Leonxlnx/taste-skill
  ```
- [**Dammyjay93/interface-design**](https://github.com/Dammyjay93/interface-design) <img src="https://img.shields.io/github/stars/Dammyjay93/interface-design?style=flat-square&logo=github&label=" height="16"> — 持久設計系統記憶 + `/interface-design:audit` 斜線指令
  ```sh
  git clone https://github.com/Dammyjay93/interface-design ~/.claude/plugins/interface-design
  ```
- [**coleam00/excalidraw-diagram-skill**](https://github.com/coleam00/excalidraw-diagram-skill) <img src="https://img.shields.io/github/stars/coleam00/excalidraw-diagram-skill?style=flat-square&logo=github&label=" height="16"> — 用視覺論證的圖表；渲染—驗證循環
  ```sh
  git clone https://github.com/coleam00/excalidraw-diagram-skill .claude/skills/excalidraw-diagram
  ```
- [**OneRedOak/claude-code-workflows**](https://github.com/OneRedOak/claude-code-workflows/tree/main/design-review) <img src="https://img.shields.io/github/stars/OneRedOak/claude-code-workflows?style=flat-square&logo=github&label=" height="16"> — Patrick Ellis 的 design-review 子代理 + `/design-review` + CLAUDE.md 摘錄；需要 Playwright MCP
  ```sh
  git clone https://github.com/OneRedOak/claude-code-workflows
  cp -r claude-code-workflows/design-review/.claude/* .claude/
  ```
- [**ComposioHQ/awesome-claude-skills — canvas-design**](https://github.com/ComposioHQ/awesome-claude-skills/tree/master/canvas-design) <img src="https://img.shields.io/github/stars/ComposioHQ/awesome-claude-skills?style=flat-square&logo=github&label=" height="16"> — 設計哲學 → 海報/PDF 成品，兩階段
  ```sh
  npx skillkit install composio/canvas-design
  ```
- [**Owl-Listener/designer-skills**](https://github.com/Owl-Listener/designer-skills) <img src="https://img.shields.io/github/stars/Owl-Listener/designer-skills?style=flat-square&logo=github&label=" height="16"> — [Marie-Claire Dean 的 63 技能 + 27 指令 + 8 外掛](https://marieclairedean.substack.com/p/i-built-63-design-skills-for-claude)，MIT — 涵蓋研究、系統、策略、UI、互動、原型、營運，以及工具包本身
  ```sh
  /plugin marketplace add Owl-Listener/designer-skills
  ```
- [**Snyk — UI/UX 工程師的 8 大 Claude 技能**](https://snyk.io/articles/top-claude-skills-ui-ux-engineers/) — 第三方彙整；解說 frontend-design 技能（277k+ 安裝）、`ui-ux-pro-max` 與 Vercel 配套技能，附安裝指令
- [**Snyk — 創業者／創辦人的 8 大 Claude 技能**](https://snyk.io/articles/top-8-claude-skills-entrepreneurs-startup-founders-solopreneurs/) — 配套彙整；為單人建構者框定設計相關技能，捕捉社群從「這會取代我嗎」轉向「我怎麼更快出貨」的心態變化

## 整合

可與 Claude Design 搭配、或透過 Claude Code 交接延伸它的 MCP 伺服器、外掛與 IDE 轉接器。多數存在於產品介面之外 — 接好一次，之後就把 Claude Design 的匯出路由過去。

### MCP 伺服器

- [**透過 MCP 把 Claude Code 連到工具**](https://code.claude.com/docs/en/mcp) — 官方設定文件、scope、傳輸模式
- [**Figma MCP 伺服器**](https://www.figma.com/blog/introducing-figmas-dev-mode-mcp-server/) — 橋接設計到程式碼；補上 Claude Design 發布時缺的 Figma 匯出
- [**Adobe AEM MCP**](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/mcp-support/chat-applications/setup-claude) — Claude + AEM 設定教學，從聊天進行內容撰寫

### 精選 MCP 彙整

- [**TurboDocx — 最佳 Claude Code 外掛/技能/MCP**](https://www.turbodocx.com/blog/best-claude-code-skills-plugins-mcp-servers) — 外掛/技能/伺服器合併清單，有主見的精選
- [**claudefa.st — 50+ 最佳 MCP 伺服器**](https://claudefa.st/blog/tools/mcp-extensions/best-addons) — 帶分類標籤的廣泛目錄
- [**Builder.io — 如何使用 MCP 伺服器**](https://www.builder.io/blog/claude-code-mcp-servers) — 安裝 + 設定模式，附範例
- [**Toolradar — 2026 最佳 MCP 伺服器**](https://toolradar.com/blog/best-mcp-servers-claude-code) — 排名清單，附工作流程備註
- [**LaoZhang — 依工作流程的入門精選**](https://blog.laozhang.ai/en/posts/claude-code-best-mcp-servers) — 依用例分類（研究、編碼、基礎設施）
- [**MindStudio — 透過 MCP 讀寫 app**](https://www.mindstudio.ai/blog/how-to-use-mcp-servers-with-claude-code) — 把第三方 app 變成 MCP 可讀介面

### 前沿功能

Claude Design 內建了過去需要另外工具的 AI 輸出 — **語音、影片、3D、Shader** 全部行內生成（出自 [Anthropic 發布文](https://www.anthropic.com/news/claude-design-anthropic-labs)）。Connectors（Slack、Drive、內部文件）無需額外 MCP 接線就能插進設計循環；槓桿高，但燒額度也快。

### 透過 MCP 串接 Stitch + Claude Design

- [**Pasquale Pillitteri — Google Stitch MCP，把 Claude Code 設計匯出成程式碼**](https://pasqualepillitteri.it/en/news/647/google-stitch-mcp-export-claude-code-design-to-code) — 完整的 Stitch + CD 經 MCP 教學。涵蓋 Stitch 2026 年 3 月更新（Vibe Design、Voice Canvas、多畫面流程、每月 350 次免費生成）與透過 MCP 接進 Claude Code、Cursor 或 Gemini CLI 的 React/Vue/Angular/Flutter/SwiftUI 匯出。

### Canva 整合

- [**Canva newsroom — Canva 與 Claude Design**](https://www.canva.com/newsroom/news/canva-claude-design/) — Canva 方的官方合作公告
- [**Morningstar / BusinessWire — Canva 宣布與 Anthropic 合作**](https://www.morningstar.com/news/business-wire/20260410843169/canva-announces-anthropic-collaboration-to-bring-ai-powered-design-to-millions) — 4/10 新聞稿，在 Krieger 辭去 Figma 董事四天前、發布七天前
- 根據 [Lalindra 在 Pen With Paper 的實測](https://medium.com/pen-with-paper/claude-design-review-i-spent-a-day-with-it-heres-what-actually-happens-441922202ef2)，Claude Design「部分由」Canva Foundation Design Model 驅動，並支援 HTML 匯入，可把 Canva 做的版面回送到編輯器來回往返。

### 企業／Cowork 管理

- [**Anthropic — Team 與 Enterprise 方案的 Claude Design 管理指南**](https://support.claude.com/en/articles/14604406-claude-design-admin-guide-for-team-and-enterprise-plans) — 官方 4 階段推行（設計師 → 整個設計團隊 → 更廣 → 全組織）、自訂角色、設計系統先行的順序，以及資料落地（data residency）注意事項（CD 目前不支援落地需求）
- [**Anthropic — Claude Cowork 企業管理員指南**](https://claude.com/resources/tutorials/claude-cowork-enterprise-administrator-guide) — 相鄰的管理脈絡，涵蓋與 CD 佈建交叉的 Cowork 側控制

### 須知的限制

- **發布時尚無 Figma 匯出** — 回送 Figma 需手動；token 同步請用上面的 Figma MCP 伺服器
- **無即時游標多人協作** — 產品沒有 Figma 式的共同編輯
- **分享是組織範圍 URL，只有檢視/編輯** — 沒有公開連結、沒有逐元素權限
- **推斷的設計系統可能誤判邊緣案例** — 自動擷取的 tokens 在離群值上會漂移；鎖定前先審查（[agence-scroll 指南](https://agence-scroll.com/en/blog/claude-design-anthropic-2026-guide)）

## 工作流程與食譜

端到端流程在 `/recipes/<name>.md`。

1. [**20 分鐘登陸頁**](recipes/landing-page-20-min.md) — DESIGN.md → Claude Design → Claude Code → Vercel
2. [**Figma 檔案 → DESIGN.md**](recipes/figma-to-design-md.md) — 把 `.fig` 拖進聊天、擷取 tokens、重用
3. [**現有倉庫 → 設計系統**](recipes/repo-to-design-system.md) — 把 Claude 指向你的 CSS，取回標準 DESIGN.md
4. [**線框 → 高保真**](recipes/wireframe-to-hifi.md) — 低保真草圖到像素完美稿
5. [**從 README 做簡報**](recipes/pitch-deck-from-readme.md) — 從專案 README 做 12 頁簡報
6. [**品牌擷取**](recipes/brand-extraction.md) — URL → 描述競品系統的 DESIGN.md
7. **設計系統治理** — 把 tokens 鎖成 `SKILL.md`，供日後每個專案使用
8. [**網頁擷取 → 原型**](recipes/web-capture-to-prototype.md) — 在你的線上網站用原生擷取工具
9. **16 分鐘全部做完** — 引用 @petergyang：影片＋簡報＋網站＋app ＋初始系統
10. **雙品牌混搭** — 一致地結合兩個 DESIGN.md 的 tokens
11. **Claude Design → Canva 匯出** — 設計師協作路徑
12. **全組織設計系統分享** — 唯讀 URL、群組聊天編輯模式
13. [**Claude Design 的 Token 預算**](recipes/token-budget-claude-design.md) — 用單一 Pro 方案在一週內出貨一個專案而不燒爆額度
14. [**前沿 3D / shader / 語音 / 影片**](recipes/frontier-3d-shaders.md) — 用 Claude Design 的原生生成介面建構；引用 Anthropic 發布文＋ Ileana Marcut 的 3D Helix 作品集
15. [**Tweaks 面板 — 不重新生成的迭代**](recipes/tweaks-panel-sidebar.md) — 重新排序章節、替換變體，不燒聊天 token；Austin Lau 的側欄工作流程
16. [**註解貼上變通法**](recipes/comment-paste-workaround.md) — 把本來要打進聊天的提示詞貼成行內註解；MacStories 的「95%」模式
17. [**從簡報抽出講者備註**](recipes/speaker-notes-pitch-deck.md) — 從生成的簡報抽出可直接上場的備註；與 `pitch-deck-from-readme` 搭配

<p align="center"><img src="assets/mascot.svg" width="72" alt="mascot"></p>

## 長篇教學

塵埃落定後值得讀的文章。依平台分組。

### Substack

| 標題 | 作者 | URL | 價值 |
|---|---|---|---|
| Claude Design is here | Department of Product | [departmentofproduct.substack.com](https://departmentofproduct.substack.com/p/claude-design-is-here-everything) | 5 個範例 + GitHub 模擬設定 + 聊天 vs 註解之分 — 最實戰的第一小時指南 |
| Claude Design | Ruben Hassid | [ruben.substack.com](https://ruben.substack.com/p/claude-design) | 管理員開關設定步驟 + 進階工作流程 |
| Founder's Playbook | Linas Beliūnas | [linas.substack.com](https://linas.substack.com/p/claude-design-founders-playbook) | 八種工作流程、7 步驟 logo 流程、master prompts；引用 Mercury 90% 推論 |
| How to Actually Use Claude Design | AI For Developers | [aifordevelopers.substack.com](https://aifordevelopers.substack.com/p/how-to-actually-use-claude-design) | 完整的「子目錄而非 monorepo」訣竅 |
| Claude for Designers Ultimate Guide | Sorted Pixels (nervegna) | [nervegna.substack.com](https://nervegna.substack.com/p/claude-for-designers-the-ultimate) | 三級模型：新手 / 實作者 / 編排者 |
| Solopreneur Initial Guide | solopreneurcode | [solopreneurcode.substack.com](https://solopreneurcode.substack.com/p/claude-design-complete-guide-solopreneurs) | 單人創辦人尺度，無代理商假設 |
| Everything You Need to Know | getpushtoprod | [getpushtoprod.substack.com](https://getpushtoprod.substack.com/p/everything-you-need-to-know-about) | 四範本工作流程：原型 / 投影片 / 範本 / 其他 |
| I Tested It On Launch Day | aifromthefield | [aifromthefield.substack.com](https://aifromthefield.substack.com/p/i-tested-claude-design-on-launch) | 第一天實測，在輿論收斂之前 |
| What Claude Design is actually good for | Lenny's Newsletter | [lennysnewsletter.com](https://www.lennysnewsletter.com/p/what-claude-design-is-actually-good) | 登陸頁 + 投影片 + 「失控改版」壓力測試 |

### Medium

| 標題 | 作者 | URL | 價值 |
|---|---|---|---|
| I Spent a Day With It — Here's What Actually Happens | Lalindra (Pen With Paper) | [medium.com/pen-with-paper](https://medium.com/pen-with-paper/claude-design-review-i-spent-a-day-with-it-heres-what-actually-happens-441922202ef2) | 揭露 Canva Design Engine 夥伴關係；非設計師視角 |
| What Claude Design actually changes for designers | Fanny | [medium.com/design-bootcamp](https://medium.com/design-bootcamp/what-claude-design-actually-changes-for-designers-0c5b04fae343) | 簡報 → Claude Code 管線塌縮，設計師視角 |
| What's New, What You Can Build, How to Use It | Ai Studio | [medium.com/the-ai-studio](https://medium.com/the-ai-studio/claude-design-whats-new-what-you-can-build-and-how-to-use-it-92283bfe8c82) | 涵蓋三大產品介面的概覽掃描 |
| The Non-Designer's Walkthrough | Alex P. | [medium.com/@0xmega](https://medium.com/@0xmega/how-to-use-claude-design-the-non-designers-walkthrough-2adc18053a5c) | 六條匯出路徑，端到端 |
| Designer's First Walkthrough | Abhi Chatterjee | [designsystemscollective.com](https://www.designsystemscollective.com/claude-design-just-launched-a-designers-first-walkthrough-c79d7ce47b9b) | 「一套設計系統＋一個原型燒掉 50% 週額度」 |
| Full Breakdown | Victoria Okwuokenye | [medium.com/design-bootcamp](https://medium.com/design-bootcamp/claude-design-is-here-full-breakdown-a32767258fb9) | 逐章節的產品導覽 |
| Google makes DESIGN.md open source | fernandocomet | [medium.com/design-bootcamp](https://medium.com/design-bootcamp/google-makes-design-md-open-source-on-its-way-to-become-a-industry-standard-16119f2368dd) | DESIGN.md 規格脈絡 — 採用前先讀 |

### 部落格／其他

| 標題 | 作者 | URL | 價值 |
|---|---|---|---|
| Hands-on with Anthropic Labs' Claude Design Preview | John Voorhees (MacStories) | [macstories.net](https://www.macstories.net/stories/hands-on-with-anthropic-labs-claude-design-preview/) | Apple 媒體視角 —「對元素留言涵蓋 95% 所需」 |
| Claude Design Hands-on Review | LLMx Blog | [llmx.tech](https://llmx.tech/blog/claude-design-hands-on-review-2026/) | 「第一個行為像設計師在迭代的 AI 設計介面」 |
| How to Use Claude Design for UX/UI | DesignerUp | [designerup.co](https://designerup.co/blog/how-to-use-claude-design-for-ux-ui/) | 給對設計好奇的開發者的教學框架 |
| Getting Started | Muzli | [muz.li/blog](https://muz.li/blog/getting-started-with-claude-design-a-collaborator-for-your-design-workflow/) | 設計師電子報式入門，低門檻上手 |
| Good Enough for Professional Websites? | BSWEN | [docs.bswen.com](https://docs.bswen.com/blog/2026-04-18-claude-design-quality-professional/) | 品質門檻誠實評估，偏懷疑 |
| The Visual Layer Claude Code Was Missing | Mejba Ahmed | [mejba.me](https://www.mejba.me/blog/claude-design-visual-workflow-claude-code) | 工程師正面解讀；與 Claude Code 工作流程搭配 |
| 15 Minutes to a Design System | Ocasio Consulting | [ocasioconsulting.com](https://ocasioconsulting.com/claude-design-review/) | 直接向 Anthropic 要固定設計席位費 |
| Complete Guide | Tosea.ai | [tosea.ai/blog](https://tosea.ai/blog/claude-design-complete-guide) | 參考文件形態；適合作為深連結目標 |
| First Impressions | Banani | [banani.co/blog](https://www.banani.co/blog/claude-design-review) | 競品的評測 — 帶著這點讀 |
| Anthropic's Answer to Lovable / v0 | Aurora Designs | [aurora-designs.ca](https://aurora-designs.ca/blog/claude-design-anthropic-labs/) | 把 Claude Design 放進 AI 建構器領域定位 |
| Complete 2026 Guide | agence-scroll | [agence-scroll.com](https://agence-scroll.com/en/blog/claude-design-anthropic-2026-guide) | 代理商側的採用框架 |
| Complete Guide for Non-Designers | BuildFastWithAI | [buildfastwithai.com](https://www.buildfastwithai.com/blogs/claude-design-anthropic-guide-2026) | 明確的非設計師鷹架 |
| 2026 Business Guide | Spicy Advisory | [spicyadvisory.com](https://www.spicyadvisory.com/blog/claude-design-anthropic-labs-guide-workflows-2026) | 給 SMB／顧問情境的工作流程 |
| Features + Pricing | ALM Corp | [almcorp.com](https://almcorp.com/blog/claude-design-anthropic-labs/) | 樸實的定價/功能摘要，少廢話 |

## 國際報導

值得追蹤的非英語報導。不同角度、不同受眾 — 既利於觸及翻譯讀者，也因為區域媒體常挖出美國中心浪潮錯過的角度。

### 法語

| 來源 | URL | 價值 | 語言 |
|---|---|---|---|
| La Revue Tech | [larevuetech.fr](https://larevuetech.fr/anthropics-claude-design-wants-to-turn-a-prompt-into-a-prototype-then-hand-it-to-canva-or-code/) | 提示詞到原型框架，帶 Canva/Code 交接角度 | FR |
| IT SOCIAL | [itsocial.fr](https://itsocial.fr/contenus/actualites/intelligence-artificielle-actualites-contenus/avec-claude-design-anthropic-ouvre-le-prototypage-visuel-aux-professionnels-sans-competences-en-crea/) | 企業 IT 視角 — 向非創意專業者開放視覺原型 | FR |

### 西語

| 來源 | URL | 價值 | 語言 |
|---|---|---|---|
| Web Reactiva | [webreactiva.com](https://www.webreactiva.com/blog/claude-design-probado) | 西語實測；測了 Claude Code 匯出路徑 | ES |

### 義語

| 來源 | URL | 價值 | 語言 |
|---|---|---|---|
| Pasquale Pillitteri — Vibe Coding 2026 比較 | [pasqualepillitteri.it](https://pasqualepillitteri.it/en/news/591/ai-app-builders-comparison-2026) | 詳細的 AI app 建構器比較，含 Claude Design 定價爭議 | IT（英文翻譯） |
| Pasquale Pillitteri — CD vs Stitch 股災分析 | [pasqualepillitteri.it](https://pasqualepillitteri.it/en/news/1027/claude-design-vs-google-stitch-figma-stock-crash) | 義語分析 Figma 股災 + Stitch 定位 | IT（英文翻譯） |
| Pasquale Pillitteri — Stitch MCP 教學 | [pasqualepillitteri.it](https://pasqualepillitteri.it/en/news/647/google-stitch-mcp-export-claude-code-design-to-code) | 23 分鐘完成 Stitch MCP Server + Claude Code 設計到程式碼流程 | IT（英文翻譯） |

### 日語

| 來源 | URL | 價值 | 語言 |
|---|---|---|---|
| 金 成奎（seikei_kin）on X | [x.com/seikei_kin](https://x.com/seikei_kin/status/2032264221644505561) | 把 Marie-Claire Dean 的 63 技能整理翻成日文並放大給日本受眾 | JA |

歡迎發 PR 加入更多國際來源 — 韓語、中文、德語、葡語與其他區域報導都是我們想補的缺口。開 issue 或 PR，附上 URL、語言標籤與一行價值說明。

## 訣竅與技巧

來自真正用它出貨的創作者的高槓桿戰術。每條主張都附出處。

### Ryan Mather 的 7 個訣竅（[討論串](https://x.com/Flomerboy/status/2045162321589252458) · [Skills 說明](https://x.com/Flomerboy/status/2034094212161945965)）

Anthropic 內部人，發布第二天發布。

1. **系統先行。** 在做任何原型之前先建好設計系統 — Claude 會在之後每個成品重用 tokens。
2. **用註解，別用聊天。** 畫布上的行內註解比新開一輪聊天更省、更精準。
3. **用影片示範。** 把螢幕錄影丟進脈絡；Claude 跟隨動態意圖比看文字規格更準。
4. **接 Slack 與文件 connectors。** 接好你的知識來源，讓品牌語氣與文案保持一致（燒額度快 — 見下方週額度說明）。
5. **打造一次性小工具。** Claude 能為某個確切的微任務生出小工具，免得你跟一個通用工具搏鬥。
6. **在關鍵時刻放慢。** 主視覺、定價、空狀態 — 讓 Claude 在那多跑幾趟，其他地方少跑。
7. **技能化。** 把可用的 `DESIGN.md` 打包成 `SKILL.md` 跨專案重用 — 它解鎖了什麼，見 Skills 說明討論串。

### 值得研究的建構者範例

- **Ran Segall — 自學教育 app。** 稱 Claude Design 在做完整 app 上「比 Lovable 或 Replit 好 10 倍」。看他的時間軸了解提示詞節奏。
- **Jerrod Lew — 兩個提示詞做出個人儀表板 OS。** 展示一個好的 `DESIGN.md` 能帶你走多遠。
- **[Peter Yang — 16 分鐘全部做完](https://x.com/petergyang/status/2045527271650558383)。** 影片＋簡報＋網站＋app ＋設計系統。也是「好玩但很快燒光用量」的出處。
- **[Austin Lau（Anthropic 成長行銷）— Tweaks 面板 + Cowork 登陸頁重現](https://x.com/helloitsaustin/status/2045176910569980318)。** 不重新生成側欄工作流程的最佳紀錄 — 重排章節、替換變體，再交接給 Claude Code。

### Token 經濟學

- **[Quasa.io — Claude Design token 訣竅](https://www.quasa.io/)** — 社群整理的額度求生；與 [`token-budget-claude-design`](recipes/token-budget-claude-design.md) 配方搭配。
- **促銷額度會先被消耗。** Anthropic 給每個付費使用者一次性、約等於一個典型 $20 提示詞的額度；拿去實驗，把週額度留給正式工作。
- **週額度依使用者計算，非共用池。** 規劃團隊用量時很重要 — 管理員無法重新分配別人剩餘的預算。
- 以上兩點皆出自 [Anthropic — Claude Design 訂閱用量與定價](https://support.claude.com/en/articles/14667344-claude-design-subscription-usage-and-pricing)。

### 工作流程要點

- **接 Slack 與文件 connectors** 是品牌一致性槓桿最高的整合，但也是最快燒光週額度的方式。只在正式專案接，別在探索階段接。
- **子目錄，不是 monorepo。** 根據 [AI For Developers](https://aifordevelopers.substack.com/p/how-to-actually-use-claude-design)，每個專案把 Claude Design 指向單一子目錄 — 整個 monorepo 的脈絡又慢又雜。每個 app 一個 `DESIGN.md`，從子目錄連結。

## Podcast 報導

值得排進清單的音訊報導。內部人訪談、發布週反應，以及來自 v0／生成式網頁圈的相鄰脈絡。

- [Lenny's Podcast — Jenny Wen（Claude 設計負責人、前 Figma 總監），「設計流程已死」](https://www.lennysnewsletter.com/p/the-design-process-is-dead) — 核心集（2026 年 3 月 1 日，1 小時 17 分）。早於發布，但奠定哲學基礎：探索 → 模擬 → 迭代已死、Anthropic 招募的三種設計師原型、AI 品味/判斷、她為何離開 Figma 總監回到 Anthropic 當 IC。
- [Lenny's Newsletter 迷你集（4/22）—「Claude Design 到底擅長什麼」](https://www.lennysnewsletter.com/p/what-claude-design-is-actually-good) — 發布後反應。配套 YouTube：[「Claude Design 很慢但我還是愛它」](https://www.youtube.com/watch?v=wgPVh9wG6Ok)。登陸頁＋投影片＋失控改版測試；CD + GPT Images 2.0 + DESIGN.md 並列。
- [AI Daily Brief（Nathaniel Whittemore）— Claude Design 集](https://podcasts.apple.com/us/podcast/the-ai-daily-brief-artificial-intelligence-news/id1680633614) — 最大的每日 AI podcast 報導 CD；觸及非設計的 AI 受眾。前幾天最佳用例；行銷／簡報／線框／發布影片。配套 [Claude Cowork 集](https://open.spotify.com/episode/5krjdNlepb26fNWmcsRjG9)。
- [Design Better Podcast —「The Roundup：我們對 Claude Design 的第一印象」](https://designbetterpodcast.com/p/the-roundup-our-first-impressions) — 設計師主持人圓桌。「有趣的問題不是生成像素 — 是生成看起來像 *你的* 產品的像素。」「還不是 Figma 殺手」的解讀。
- [Design Better Podcast — Meaghan Choi（Anthropic 在 Claude Code 的產品設計師）](https://www.designbetter.co/podcast) — 相鄰脈絡：Anthropic 設計師對更廣 Claude 產品介面的觀點（確切集數待定）。
- [Sequoia Training Data — Vercel CEO Guillermo Rauch：用 AI 打造生成式網頁](https://sequoiacap.com/podcast/training-data-guillermo-rauch/) — 同一波浪潮中 v0／生成式網頁側的相鄰脈絡。
- [Lenny's Podcast —「現在人人都是工程師：v0 的使命內幕」（Guillermo Rauch）](https://www.lennysnewsletter.com/p/everyones-an-engineer-now-guillermo-rauch) — Rauch 集；v0 框架對比較內容有用。
- [AI and I — Vercel 的 Guillermo Rauch 談編碼之後是什麼](https://creators.spotify.com/pod/profile/how-do-you-use-chat-gpt/episodes/Vercels-Guillermo-Rauch-on-What-Comes-After-Coding---Ep--47-e2tguf3) — 第三個 Rauch 觀點；補足 Sequoia ＋ Lenny 兩集。
- [How I AI —「給產品經理的 Claude Code」](https://www.lennysnewsletter.com/p/this-week-on-how-i-ai-claude-code) — 相鄰的 PM 視角脈絡；CC 觀點適用於 CD 工作流程。

## 常見問題

**Claude Design 會取代 Figma 嗎？**
今天不會。它取代的是初稿階段（線框、視覺稿、簡報）。團隊仍會經由 Figma 來回做協作、開發交接、外掛。

**一定要 Opus 4.7 嗎？**
發布時即綁定。Sonnet 4.6 可用，但產出的系統較弱。長任務的幻覺回報是真的。

**能匯入 Figma 檔案嗎？**
能 — 把 `.fig` 拖進聊天。單頁效果好；多檔案資料庫在發布時時好時壞。

**價格？**
綁在 Pro / Max / Team / Enterprise。每席位的 Team 定價尚未公布。

**我會燒爆 Pro 額度嗎？**
幾乎一定會，如果你每個改動都用聊天提示。Reddit 上「兩個提示吃掉 95% 週上限」的回報是真的 — Opus 4.7 視覺 token 約為等量文字的 3 倍。用 [`token-budget-claude-design`](recipes/token-budget-claude-design.md) 配方：一次搭好骨架、上限 4 張參考畫面、改用行內註解迭代、用分支做變體、一次打包到 Claude Code。Claude Design 有與聊天分開的額度 — 但如果你也用 Claude Code，那個額度是共用的。

**會拿去訓練資料嗎？**
依 Anthropic 政策：付費等級預設不會。處理敏感工作前請在 [anthropic.com/legal/privacy](https://www.anthropic.com/legal/privacy) 上確認。

**影片？**
有。引用 @petergyang：「做出的影片很漂亮，比簡報更出色。」Greg Isenberg 沒那麼驚艷。自己試了再決定。

**開源替代品？**
[SuperDesign](https://github.com/superdesigndev/superdesign) — 在你的 IDE 內執行，MIT，自帶模型。

**GitHub 上的 `anthropic-claude-design/claude-design` 是真的嗎？**
不是。假冒倉庫。Claude Design 在 [claude.ai/design](https://claude.ai/design)，需付費登入。沒有任何下載存在。

## 相關開源專案

| 倉庫 | 星數 | 是什麼 |
|---|---|---|
| [superdesigndev/superdesign](https://github.com/superdesigndev/superdesign) | <img src="https://img.shields.io/github/stars/superdesigndev/superdesign?style=flat-square&logo=github&label="> | IDE 內的開源 AI 設計代理，MIT |
| [jonthebeef/superdesign-mcp-claude-code](https://github.com/jonthebeef/superdesign-mcp-claude-code) | <img src="https://img.shields.io/github/stars/jonthebeef/superdesign-mcp-claude-code?style=flat-square&logo=github&label="> | 把 SuperDesign 當 Claude Code MCP，免 API key |
| [Owl-Listener/designer-skills](https://github.com/Owl-Listener/designer-skills) | <img src="https://img.shields.io/github/stars/Owl-Listener/designer-skills?style=flat-square&logo=github&label="> | MC Dean 的 Designer Skills Collection，MIT |
| [Owl-Listener/designpowers](https://github.com/Owl-Listener/designpowers) | <img src="https://img.shields.io/github/stars/Owl-Listener/designpowers?style=flat-square&logo=github&label="> | 專家設計代理，Direct + Auto 模式，MIT |
| [VoltAgent/awesome-claude-design](https://github.com/VoltAgent/awesome-claude-design) | <img src="https://img.shields.io/github/stars/VoltAgent/awesome-claude-design?style=flat-square&logo=github&label="> | 品牌 DESIGN.md 目錄，依產業分類 |
| [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | <img src="https://img.shields.io/github/stars/VoltAgent/awesome-design-md?style=flat-square&logo=github&label="> | Stitch 格式 DESIGN.md 收藏 |
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | <img src="https://img.shields.io/github/stars/VoltAgent/awesome-agent-skills?style=flat-square&logo=github&label="> | 技能，含 `design-md`、`shadcn-ui`、`react-components` |
| [saifyxpro/ui-ux-design-pro-skill](https://github.com/saifyxpro/ui-ux-design-pro-skill) | <img src="https://img.shields.io/github/stars/saifyxpro/ui-ux-design-pro-skill?style=flat-square&logo=github&label="> | 風格、色盤、字體、CLI |
| [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | <img src="https://img.shields.io/github/stars/nextlevelbuilder/ui-ux-pro-max-skill?style=flat-square&logo=github&label="> | 跨平台 UI/UX 技能 |
| [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | <img src="https://img.shields.io/github/stars/alirezarezvani/claude-skills?style=flat-square&logo=github&label="> | 橫跨工程、產品、行銷的技能 |
| [daymade/claude-code-skills](https://github.com/daymade/claude-code-skills) | <img src="https://img.shields.io/github/stars/daymade/claude-code-skills?style=flat-square&logo=github&label="> | Claude Code 技能市集 |
| [abhishekray07/claude-md-templates](https://github.com/abhishekray07/claude-md-templates) | <img src="https://img.shields.io/github/stars/abhishekray07/claude-md-templates?style=flat-square&logo=github&label="> | CLAUDE.md + 規則最佳實務 |
| [smartwhale8/claude-playbook](https://github.com/smartwhale8/claude-playbook) | <img src="https://img.shields.io/github/stars/smartwhale8/claude-playbook?style=flat-square&logo=github&label="> | 正式環境 `.claude/` GitHub 範本 |
| [NicholasSpisak gist](https://gist.github.com/NicholasSpisak/7cb9db221b0b7c4c4aaf9ffca21a847c) | — | 三設計師辯論提示詞 |
| [anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks) | <img src="https://img.shields.io/github/stars/anthropics/claude-cookbooks?style=flat-square&logo=github&label="> | 官方 Anthropic notebooks |
| [rohitg00/awesome-claude-plugins](https://github.com/rohitg00/awesome-claude-plugins) | <img src="https://img.shields.io/github/stars/rohitg00/awesome-claude-plugins?style=flat-square&logo=github&label="> | Claude Code 外掛生態系 |
| [rohitg00/awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit) | <img src="https://img.shields.io/github/stars/rohitg00/awesome-claude-code-toolkit?style=flat-square&logo=github&label="> | Hooks、skills、斜線指令 |
| [rohitg00/skillkit](https://github.com/rohitg00/skillkit) | <img src="https://img.shields.io/github/stars/rohitg00/skillkit?style=flat-square&logo=github&label="> | 跨多代理的通用技能 CLI |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | <img src="https://img.shields.io/github/stars/hesreallyhim/awesome-claude-code?style=flat-square&logo=github&label="> | 一般 Claude Code 資源 |
| [github.com/topics/claude-design](https://github.com/topics/claude-design) | — | 即時主題流 |

## 標籤系統

跨 `DESIGN.md`、提示詞包、食譜與混搭檔案使用的行內標籤徽章。歡迎自由分叉與混搭 — 原始檔在 [`/assets/tags/`](assets/tags/)。

<p align="center">
  <img src="assets/tags/anthropic.svg" alt="Anthropic">
  <img src="assets/tags/official.svg" alt="official">
  <img src="assets/tags/curated.svg" alt="curated">
  <img src="assets/tags/community.svg" alt="community">
  <img src="assets/tags/open-source.svg" alt="open source">
  <img src="assets/tags/new.svg" alt="new">
  <img src="assets/tags/remix.svg" alt="remix">
  <img src="assets/tags/hype.svg" alt="hype">
  <img src="assets/tags/skeptic.svg" alt="skeptic">
</p>

## 參與貢獻

標準：**一個在職設計師或工程師，會在接下來 48 小時內覺得這有用嗎？**

**接受：** 任何美學家族的原創 DESIGN.md 檔案 · 混搭配方（雙品牌組合）· 附前後截圖的提示詞包 · 你真的跑過的工作流程食譜 · 觀看數 > 2K 或有實質批評的影片拆解 · 附出處的比較資料 · 附連結與互動數的 X 帳號引言 · 真實輸出的截圖/GIF。

**拒絕：** 聯盟行銷連結 · 沒有可重現提示詞的截圖 ·「好酷喔！」沒有脈絡 · 重新包裝的 VoltAgent 條目（請連到上游）· 罐頭內容 · 大量 emoji 的標題 · 假冒倉庫。

**PR 範本：** 標題 `[family] brand — 一行價值`。內文＝色票＋字體＋參考連結＋可重現性備註。

見 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 授權

[MIT](LICENSE)。使用、分叉、混搭、出貨。

與 Anthropic 無任何關聯。「Claude」與「Claude Design」是 Anthropic PBC 的商標。所引用 DESIGN.md 檔案中的品牌名稱屬於各自所有者 — 僅作教育性評論之用。

---

<p align="center"><img src="assets/divider.svg" width="600" alt="divider"></p>

<p align="center"><img src="assets/mascot.svg" width="96" alt="mascot"></p>

<p align="center">
  由 <a href="https://github.com/rohitg00">@rohitg00</a> 維護。歡迎 PR。
</p>
