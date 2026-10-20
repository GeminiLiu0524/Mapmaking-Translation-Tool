# 翻譯鍵工作台 · Mapmaking Translation Tool

從 Minecraft 地圖或資源包提取翻譯鍵，並排比對各語言、編輯文字、§ 格式碼與地圖文字元件的顏色。

Extract translation keys from Minecraft maps and resource packs, compare languages side by side, and edit text, § format codes, and text-component colors.

## 功能

- 讀取地圖資料夾、世界 .zip、資源包（資料夾或 .zip）與單獨的語言檔
- 語言檔格式：`.json`、舊版 `.lang`、`.yml` / `.yaml`（巢狀 YAML 會攤平成以「.」連接的鍵；匯出時保留註解、空行與引號樣式）
- 掃描 `.mcfunction`、JSON / SNBT、區域檔（`.mca`）與結構（`.nbt`），找出地圖實際使用的鍵
- 標出缺翻譯、與基準相同、佔位符不符、格式碼不同、地圖使用但未定義、地圖未使用
- 遊戲預覽（§ 色碼、粗體、斜體、亂碼等），並套用地圖文字元件的 `color`
- 在地圖的 mcfunction / JSON 中直接修改文字元件的 hex 顏色
- 匯出：單檔下載、打包 .zip、轉換格式，或（Chrome / Edge）直接存回原檔
- 工作階段存檔與瀏覽器自動暫存
- 介面語言：繁體中文、English (US)、简体中文

所有處理都在瀏覽器內完成，檔案不會上傳到任何伺服器。

## 使用

打開網頁版，或下載 `index.html` 後直接用瀏覽器開啟（可離線使用）。

## 第三方元件

- [JSZip](https://github.com/Stuk/jszip) 3.10.1 — MIT 授權（或 GPLv3）
- [yaml](https://github.com/eemeli/yaml) 2.4.5 — ISC 授權
- [js-yaml](https://github.com/nodeca/js-yaml) 4.1.0 — MIT 授權

以上都已內嵌在 `index.html` 中。
