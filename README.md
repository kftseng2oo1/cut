# LINE 貼圖裁剪器

把一整張排好的貼圖表格圖片，依欄列自動裁成單張，去背後打包成 ZIP，符合 LINE 貼圖上架規格。

**線上使用**：https://kftseng2oo1.github.io/cut/

## 主要功能
- 上傳貼圖表格圖，自動偵測或手動設定欄數、列數、內距，即時預覽裁切線
- 兩種去背：從邊緣填色去背、門檻值去背
- 自動產生 `main.png` 主圖與 `tab.png` 分頁圖
- 每張可單獨下載，或「⬇️ 全部下載 (ZIP)」

## 使用方式
1. 上傳表格圖片
2. 調整欄列數直到裁切線對齊
3. 按「✂️ 開始裁切」，再下載 ZIP

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- Canvas 裁切與去背，JSZip（cdnjs）打包；規格參考 LINE Creators 官方指南

## 相關 repo
- [Cmt](https://github.com/kftseng2oo1/Cmt)：LINE 動態貼圖編輯器
