# biology-ii-plant-structure

選修生物 II 第二章「植物體的構造與功能」分科複習網站。

- 主軸：教用互動式教學講義 2-1、2-2
- 內容：分科筆記、課本必要圖版、六張原書心智圖、10 題原創情境自測
- 教材：互動式講義、課本、備課用書、六頁心智圖 PDF
- Vercel 輸出目錄：`dist`
- 二進位教材資產：部署 bundle 內含 17 張 PNG 與 4 份 PDF；檔名、大小與 SHA-256 見 `ASSET-MANIFEST.json`

## 本機預覽

```bash
python -m http.server 8000 -d dist
```

## Vercel

`vercel.json` 已將 `outputDirectory` 設為 `dist`。
