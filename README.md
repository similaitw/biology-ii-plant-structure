# biology-ii-plant-structure

選修生物 II 第二章「植物體的構造與功能」分科複習網站。

- 主軸：教用互動式教學講義 2-1、2-2
- 內容：分科筆記、課本必要圖版、六張原書心智圖、10 題原創情境自測
- 教材：互動式講義、課本、備課用書、六頁心智圖 PDF
- Vercel 輸出目錄：`dist`

## 專案結構

`dist/index.html`、`dist/styles.css`、`dist/app.js` 為網站程式碼。
完整部署 bundle 另包含：

- `dist/assets/mindmaps/`：6 張心智圖
- `dist/assets/textbook/`：11 張課本必要圖版
- `dist/pdfs/`：4 份教材 PDF

所有二進位資產的預期檔名、大小與 SHA-256 都列在 `ASSET-MANIFEST.json`。

> 目前 ChatGPT 的 GitHub 寫入連接器只支援 UTF-8 文字內容，因此此 repo 已推送網站程式碼與資產 manifest；大型 PNG/PDF 二進位檔需使用完整部署 bundle 上傳。

## 本機預覽

```bash
python -m http.server 8000 -d dist
```

## Vercel

`vercel.json` 已將 `outputDirectory` 設為 `dist`。
