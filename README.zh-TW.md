# Awesome Pele [![Awesome](https://awesome.re/badge.svg)](https://github.com/sindresorhus/awesome)

> 小型、同步、沒有執行期相依性的算繪器，把 Mermaid 圖轉成可用 CSS 變數調整外觀的 SVG。

[English](README.md) · [繁體中文](README.zh-TW.md)

Pele 是 [kepano](https://github.com/kepano) 撰寫的 MIT 授權 Mermaid 轉 SVG 算繪器，為 Obsidian 開發，也可在其他地方使用。它對應 Mermaid 12.1.0 內建的圖表類型，沒有執行期相依性，並用 CSS 變數為圖表設定外觀。儲存庫、網站、遊樂場、文件、安全政策與 npm 套件列在「官方」。

這份清單是獨立的社群目錄。它不是 Obsidian 官方專案，也不是由 Obsidian 或 kepano 維護。

## 目錄

- [官方](#官方)
- [命令列與工具](#命令列與工具)
- [移植與語言綁定](#移植與語言綁定)
- [代理技能與 AI](#代理技能與-ai)
- [靜態網站與文件整合](#靜態網站與文件整合)
- [元件與框架](#元件與框架)
- [編輯器與應用程式](#編輯器與應用程式)
- [學習與文章](#學習與文章)

## 官方

- [Pele](https://github.com/obsidianmd/pele) - 算繪器的原始碼儲存庫。
- [網站](https://pele.run) - 專案網站，含文件與即時範例。
- [遊樂場](https://pele.run/playground) - 在瀏覽器裡編輯 Mermaid 原始碼，並查看 Pele 畫出的 SVG。
- [範例](https://pele.run/examples) - Pele 支援的圖表類型畫廊。
- [API](https://pele.run/api) - render()、mount()、進入點與錯誤的參考文件。
- [外觀](https://pele.run/theming) - 用來調整圖表外觀的 CSS 變數、字型與類別名稱。
- [相容性](https://pele.run/compatibility) - 支援的 Mermaid 12.1.0 語法、圖表類型，以及版面配置差異。
- [安全指南](https://pele.run/security) - 關於不受信任圖表、連結、圖示、大小限制與錯誤顯示的說明。
- [安全政策](https://github.com/obsidianmd/pele/blob/main/SECURITY.md) - 如何回報 Pele 的漏洞。
- [npm 套件](https://www.npmjs.com/package/pele) - 已發佈的套件。以 `npm install pele` 安裝。

## 命令列與工具

- [@ahmedelgabri/pele-cli](https://github.com/ahmedelgabri/pele-cli) - 命令列介面，可驗證 Mermaid 圖並在不開啟瀏覽器的情況下輸出可調外觀的 SVG。
- [pele2svg](https://github.com/iriyak/pele2svg) - 把依賴 CSS 的 Pele SVG 轉成 GToolkit 與 Skia 可以繪製的純 SVG。
- [pele-animate](https://github.com/dkdev24/pele-animate) - 後處理器，讓 Pele 圖一次顯示一個步驟，並加上圖示。
- [pele-cli](https://github.com/IAL32/pele-cli) - 命令列算繪器，可輸出有主題的 SVG、自含的 HTML 頁面或 PNG。需要 Node.js 22 或更新版本。

## 移植與語言綁定

- [bezel-mermaid](https://github.com/crabtalk/bezel/tree/main/crates/mermaid#readme) - Pele 1.6.0 的 Rust 移植，不需瀏覽器或 JavaScript 引擎即可把 Mermaid 原始碼畫成 SVG。
- [pele.cpp](https://github.com/MohammadRaziei/pele.cpp) - 沒有相依性的 C++17 重寫，目標是同一份原始碼產出相同的 SVG。
- [pele-go](https://github.com/Broderick-Westrope/pele-go) - Pele 1.7.0 的 Go 移植，目標是位元組相同的 SVG，不使用 cgo，也不需要 JavaScript 執行環境。
- [pele.mbt](https://github.com/Omochice/pele.mbt) - Pele 的 MoonBit 移植，目標是產出相同的 SVG，並附一個以 WebAssembly 執行的 Typst 套件。
- [pele-rs](https://github.com/vijayksingh/pele-rs) - 獨立的 Rust Mermaid 引擎，附 Swift 與 WebAssembly 綁定，實作 Pele 1.6.0 的圖表家族。
- [peler](https://github.com/eli-daniels/peler) - R 套件，在 V8 裡執行 Pele，供 SVG 輸出、Quarto、R Markdown 與 Shiny 使用。

## 代理技能與 AI

- [oh-my-pele](https://github.com/tboydar/oh-my-pele) - 以 AI 掃描程式碼庫，產生多層架構圖，在本機用 Pele 算繪，並相容 oh-my-mermaid 的 `.omm` 檔。工作進行中。
- [pele-agent-plugin](https://github.com/ossianravn/pele-agent-plugin) - 給 Claude Code 與 Codex 使用的即時瀏覽器頁面，用 Pele 畫出計畫與架構。
- [pele-skill](https://github.com/jpmanson/pele-skill) - 代理技能，用 Pele 把 Mermaid 圖畫成 SVG，不需瀏覽器。可載入 Claude Code、Hermes Agent 與 OpenCode。
- [pele-skill](https://github.com/maitretofu/pele-skill) - OpenCode 技能，用 Pele 把 Mermaid 畫成 SVG 與 PNG，剖析錯誤時會再試一次。
- [pi-pele](https://github.com/Wade11s/pi-pele) - Pi 擴充功能，用 Pele 算繪 Mermaid，再把 SVG 點陣化成 PNG 顯示在終端機。

## 靜態網站與文件整合

- [astro-pele](https://github.com/Aaron-212/astro-pele) - Astro 整合與 Sätteri 外掛，在瀏覽器裡用 Pele 算繪 Mermaid 圖。
- [bookstack-pele](https://github.com/felixyman/bookstack-pele) - 在 BookStack 伺服器端用 Pele 算繪 Mermaid 程式碼區塊，並包含 PDF 與 HTML 匯出。
- [discourse-pele-theme-component](https://github.com/discourse/discourse-pele-theme-component) - Discourse 主題元件，用 Pele 算繪貼文與聊天裡的 Mermaid 程式碼區塊。
- [dokuwiki-pele](https://github.com/v4ltages/dokuwiki-pele) - DokuWiki 外掛，用 Pele 算繪 Mermaid 圖。
- [docusaurus-theme-pele](https://github.com/kywk/docusaurus-kit/tree/main/packages/theme-pele#readme) - Docusaurus 主題，用 Pele 把 Mermaid 圖畫成可調外觀的 SVG。
- [@erduotong/satteri-pele](https://github.com/erduotong/satteri-pele) - Sätteri 外掛，用 Pele 算繪 Mermaid 圖，靜態產生時也可以使用。
- [mdbook-pele](https://github.com/ld3z/mdbook-pele) - mdBook 前置處理器，用 Pele 算繪 Mermaid 圖。
- [pele-markdown](https://github.com/yue1123/pele-markdown) - 給 markdown-it、marked 與 remark 的建置期 Mermaid 轉 SVG 外掛，瀏覽器端不需要 JavaScript。
- [pele-rehype](https://github.com/WyattAu/pele-rehype) - Rehype 外掛，在 Astro、Starlight 與其他 unified 流程裡用 Pele 算繪 Mermaid 圍欄區塊。
- [pele-rustdoc](https://github.com/explodingcamera/pele-rustdoc) - Rust 巨集，把 Mermaid 圖嵌進 rustdoc，並在瀏覽器裡用 Pele 算繪。
- [@riebeckite/plugin-mermaid-pele](https://github.com/Rerurate514/riebeckite/tree/main/packages/plugins/mermaid-pele#readme) - 在 Riebeckite 裡用 Pele 把 Mermaid 程式碼區塊畫成靜態 SVG。
- [satteri-pele](https://github.com/minumarapid/satteri-pele) - Sätteri 外掛，在建置時用 Pele 把 Mermaid 程式碼區塊轉成 SVG。
- [slidev-addon-pele](https://github.com/arthurbm/slidev-addon-pele) - Slidev 附加元件，用 Pele 繪製 Mermaid 圖，並可逐步顯示。
- [sphinx-pele](https://github.com/python-project-templates/sphinx-pele) - Sphinx 擴充功能，用 Pele 算繪 Mermaid 指示詞、MyST 圍欄區塊與外部 Mermaid 檔案。
- [theme-pele](https://github.com/Cecilapp/theme-pele) - Cecil 元件主題，用 Pele 把頁面上的 Mermaid 圖畫成 SVG。
- [vitepress-plugin-pele](https://github.com/miswanting/vitepress-plugin-pele) - 在 VitePress 建置時用 Pele 算繪 Mermaid 圖，瀏覽器端不需要 JavaScript。

## 元件與框架

- [@bigmistqke/canon-plugin-pele](https://github.com/bigmistqke/skills/tree/main/packages/canon-plugin-pele#readme) - 把 Canon 文件的推導畫成由 Pele 算繪的圖。
- [@bobril/mdx-pele](https://github.com/bobril/mdx-pele) - 用 @bobril/pele 算繪 Bobril MDX 裡的 Mermaid 程式碼區塊。
- [@bobril/pele](https://github.com/bobril/pele) - Bobril 元件，用 Pele 把 Mermaid 語法畫成 SVG。
- [comark-pele](https://github.com/farnabaz/comark-pele) - Comark 剖析外掛，以及 HTML、ANSI、Vue、React、Svelte 與 Angular 元件，用 Pele 算繪 Mermaid。
- [@docs.plus/extension-mermaid](https://github.com/docs-plus/docs.plus/tree/main/extensions/extension-mermaid#readme) - Tiptap 擴充功能，用 Pele 把 Mermaid 程式碼區塊畫成即時 SVG。
- [@maxtune/streamdown-pele](https://github.com/MaxtuneLee/streamdown-pele) - Streamdown 轉接器，用 Pele 算繪 Mermaid 程式碼區塊。
- [streamdown-pele](https://github.com/farnabaz/streamdown-pele) - Streamdown 外掛，用 Pele 取代 @streamdown/mermaid 來算繪 Mermaid 程式碼區塊。
- [@tooee/mermaid-pele](https://github.com/gingerhendrix/tooee/tree/main/packages/mermaid-pele#readme) - 選擇性啟用的 Tooee 算繪器，用 Pele 繪製 Mermaid 圍欄區塊並點陣化，供終端機顯示。

## 編輯器與應用程式

- [Diagram Studio](https://github.com/QAbot-zh/diagram-studio) - 瀏覽器圖表工作台，可用 Mermaid 或 Pele 算繪，並匯出 SVG 或 PNG。
- [dsh-pele](https://github.com/hesheng01/dsh-pele) - DeepSeek Harness 整合，透過 pele_draw 工具接收 Mermaid，並用 Pele 顯示內嵌 SVG 卡片。
- [dsh-pele](https://github.com/Yjsmall/dsh-pele) - 用 Pele 算繪 DeepSeek Harness 助理訊息裡的 Mermaid 程式碼區塊，含主題與縮放。
- [dsh-pele-mermaid](https://github.com/Farewe1ll/dsh-pele-mermaid) - DeepSeek Harness 套件外掛，在網頁聊天中用 Pele 算繪 Mermaid，而不修改 Harness 原始碼。
- [dsh-pele-mermaid](https://github.com/lsy1998/dsh-pele-mermaid) - 在 DeepSeek Harness 網頁介面用 Pele 算繪 Mermaid 圍欄區塊，含程式碼與圖表切換，以及 SVG 匯出。
- [Eos](https://github.com/campfireshuffle/eos) - 本機優先的 Mermaid 編輯器，由 Pele 算繪，圖存在瀏覽器裡，並可透過 WebMCP 讓代理使用。
- [Kilauea](https://github.com/prdlk/kilauea) - Pele 圖的視覺編輯器。可在畫好的圖上改標籤、形狀與節點。
- [Mermaid Pele Preview](https://github.com/pdanpdan/mermaid-pele-preview) - Visual Studio Code 擴充功能，用 Pele 預覽 Mermaid 檔與 Markdown 程式碼區塊，含縮放、平移與編輯器主題。
- [Mermaid Viewer](https://github.com/mmattia09/mermaid-viewer) - 在瀏覽器與 Visual Studio Code 裡即時預覽 Mermaid 檔。預設引擎是 Pele，也可改用 Mermaid.js 對照。
- [ob-pele](https://github.com/wangjia15/ob-pele) - Obsidian 外掛，用 Pele 算繪 Mermaid 與 Pele 圍欄區塊，含主題、即時預覽與縮放。
- [Pele for Paseo](https://github.com/sojuhub/paseo-plugin-pele) - 在 Paseo 聊天裡把 Mermaid 與 Pele 圍欄區塊畫成可互動的 SVG，含縮放、平移、原始碼檢視與全螢幕。
- [pele.live](https://github.com/Akshad135/pele-live) - 瀏覽器遊樂場，在本機用 Pele 算繪 Mermaid。
- [pele-mermaid](https://github.com/xiangyuio/zcode-plugins/tree/main/plugins/pele-mermaid#readme) - ZCode 外掛，在對話裡用 Pele 把 Mermaid 圖畫成內嵌 SVG。
- [Pele Note](https://github.com/ogaogamirai/pele-note) - 單檔的 Markdown 與 Mermaid 工作室，再加上使用 Pele 的命令列 SVG 轉換器。
- [Pele Preview](https://github.com/pskchai/vscode-pele-preview) - Visual Studio Code 的 Mermaid 檔預覽，由 Pele 算繪。
- [Pele Studio](https://github.com/l-velazquez/pele-studio) - 瀏覽器編輯器，用來撰寫、預覽並匯出由 Pele 算繪的圖。
- [roam-pele](https://github.com/ujuc/roam-pele) - 在 Roam Research 裡用 Pele 算繪 Mermaid 圖，區塊寬度改變時會重新排版。
- [Siren](https://github.com/plwg/siren) - 極簡瀏覽器編輯器，用 Pele 算繪 Mermaid 圖。

## 學習與文章

- [pele.wiki](https://pele.wiki) - 獨立的 Pele 指南與即時示範。與 Obsidian 或 kepano 無關。

## 註腳

移植、語言綁定與外掛會寫明它們對應的 Pele 版本。這些目標可能落後目前的發行版。若需要位元組相同的輸出，請先查看該專案本身。

## 貢獻

開 pull request 之前請先閱讀[貢獻指南](contributing.md)（[繁體中文](contributing.zh-TW.md)）。條目有變動時，請同時更新這份繁體中文版與英文版。
