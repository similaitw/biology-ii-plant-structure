# biology-ii-plant-structure

選修生物 II 第二章「植物體的構造與功能」分科複習網站。

- 主軸：教用互動式教學講義 2-1、2-2
- 內容：分科筆記、課本必要圖版、六張原書心智圖、10 題原創情境自測
- 教材：互動式講義、課本、備課用書、六頁心智圖 PDF
- Vercel 輸出目錄：`dist`

## 專案結構

`dist/index.html`、`dist/styles.css`、`dist/app.js` 為網站程式碼。

完整部署資產已納入 repository：

- `dist/assets/mindmaps/`：6 張心智圖
- `dist/assets/textbook/`：11 張課本必要圖版
- `dist/pdfs/`：4 份教材 PDF
- `ASSET-MANIFEST.json`：資產檔名、大小與 SHA-256

二進位資產已由 Vercel production deployment 回填至 GitHub；同步流程保留於
`.github/workflows/sync-assets-from-vercel.yml`。

## 本機預覽

```bash
python -m http.server 8000 -d dist
```

## Vercel

`vercel.json` 已將 `outputDirectory` 設為 `dist`。

目前 production deployment：
https://biology-ii-plant-structure-vercel-d.vercel.app

Vercel Drop 專案名稱：
`biology-ii-plant-structure-vercel-drop`

GitHub repository：
https://github.com/similaitw/biology-ii-plant-structure
