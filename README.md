# 🏫 AI 課表查詢系統產生器 (Timetable System Generator)

這是一個由 AI 驅動的靜態網頁課表查詢系統樣板。只要您有學校的課表檔案（PDF、Excel 或 Word），交給您的 AI 助手（例如 ChatGPT, Claude 或 Gemini），並附上這個 Repo 的連結，AI 就會自動幫您將課表轉成精美的響應式查詢網站！

👉 **[線上展示網站 (Live Demo)](https://littleyi22.github.io/timetable-demo/)**

---

## 🤖 給 AI 助手的 Prompt (使用說明)

請複製以下整段指令與本 Repo 連結，並附上您的課表檔案發送給 AI 助手：

> **「請參考並使用這個 Repo：`https://github.com/littleyi22/timetable-demo` 的架構。我已經附上了我們學校的課表檔案，請幫我：**
> **1. 讀取並解析我的課表內容。**
> **2. 將解析出的課表資料寫成符合該系統格式的 `timetable_XXX.csv` 與對應的 `homerooms_XXX.json`。**
> **3. 修改前端的 `config.js` 與 `index.html`，將學校名稱換成我們學校，並將介面設定正確連結至新產生的 CSV。**
> **4. 若原本沒有安裝 Firebase 或其他靜態網頁代管，請協助我將產生的網站部署上線（例如透過 GitHub Pages 或 Firebase Hosting）。」**

---

## 專案目錄結構 (AI 參考用)
```
timetable-demo/
├── index.html              # 系統入口與前端版面佈局
├── style.css               # 樣式表（含 RWD 與光影特效）
├── app.js                  # 核心邏輯（課表渲染、CSV解析、過濾）
├── config.js               # 系統設定檔（學期設定、網頁標題）
├── timetable_sample.csv    # CSV 資料表格式範例
└── homerooms_sample.json   # 班級導師對應格式範例
```

## 功能特色
* **快速、輕量**：純前端靜態網頁（HTML/CSS/JS），無須架設後端伺服器或資料庫。
* **支援多學期**：可從 `config.js` 輕鬆切換不同學期、暑輔的課表。
* **自動支援手機版**：現代化 UI 設計，針對手機、平板與電腦螢幕皆有良好體驗。
* **提供列印功能**：網頁內建列印樣式，可直接一鍵列印紙本課表。
* **支援訪客登入**：免密碼快速進入查詢。

© 2026 奕鈞老師 版權所有 | 版本：v.1.1
