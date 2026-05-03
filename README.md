# weekgen

**MNnews 週報精選工具** — 把 MNnews 的 `feed.json` 內容用勾選方式挑出 5 則，自動產出可發表的 HTML / Markdown 週報。

## 使用方式

1. 直接打開 [`index.html`](./index.html)（或部署到 Vercel / GitHub Pages 後從網址開啟）。
2. 工具會嘗試從同目錄載入 `feed.json`。如果沒有，請按右上角「從電腦選擇 feed.json」手動上傳。
3. 用時間範圍與排序篩選後，勾選想要收錄的條目（建議 5 則）。
4. 按下「產出週報」，預覽窗格會跳出。可選擇下載 HTML、複製 HTML、或複製 Markdown。

## 輸出格式

- **HTML**：含「本期內容」目錄、每則文章的標題、來源行（內聯所有來源連結）、兩段式摘要、社群討論列表。
- **Markdown**：與 HTML 結構一致，可直接貼到 Substack、Mirror、Ghost。

## 部署

任何能提供靜態檔案的服務都行。最簡單：
- **GitHub Pages**：在 repo 設定裡開啟 Pages，Source 選 `main` branch root，網址會是 `https://astrohsu.github.io/weekgen/`。
- **Vercel**：直接 import 這個 repo，預設設定即可，網址會是 `https://weekgen.vercel.app/` 之類。
