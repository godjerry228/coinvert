# Coinvert 💱

> 支援拖曳排序、設定記憶的 iOS 風格 PWA 匯率計算機。

**Coinvert** 是一個極致輕量、專為現代瀏覽器設計的匯率換算工具。它採用 Progressive Web App (PWA) 架構，無需下載 App，即可在 iPhone 或 Android 上享有如同原生應用程式般的流暢體驗。

https://godjerry228.github.io/coinvert/ 👈 **點擊立即使用**

---

## ✨ 最新功能 (New Features)

本次更新加入了許多進階互動功能：

* **🖐 拖曳排序 (Drag & Drop)**：點擊右上角「編輯」按鈕，即可直覺地拖曳調整貨幣顯示順序。
* **⚙️ 個人化設定**：新增設定頁面，可自訂「預設貨幣」，且所有設定自動儲存 (LocalStorage)，重開網頁不流失。
* **📱 PWA 安裝整合**：內建安裝偵測，Android/Chrome 用戶可直接透過設定頁面將 App 加入主畫面。

## 🚀 核心特色

* **🍎 iOS 原生體驗**：深色模式 (Dark Mode) 設計，完美契合 iPhone 視覺風格與操作手勢。
* **⚡️ 即時匯率更新**：整合公開匯率 API，一鍵刷新獲取最新市場價格。
* **🔍 智慧搜尋**：支援代碼 (USD) 與中文名稱 (美元) 快速篩選全球貨幣。
* **🏳️ 國旗顯示**：整合 FlagCDN，提供高解析度的圓形國旗圖示。
* **🛡️ 隱私優先**：完全在瀏覽器端運行，不收集任何個人數據。

---

## 📱 如何安裝 (Installation)

### iOS (iPhone/iPad)
1.  使用 **Safari** 瀏覽器打開 [專案網址]。
2.  點擊下方中間的 **「分享」** 按鈕 (方框向上箭頭圖示)。
3.  向下滑動選單，點擊 **「加入主畫面」(Add to Home Screen)**。
4.  點擊右上角的 **「新增」**。

### Android / Desktop (Chrome/Edge)
1.  使用瀏覽器打開網址 https://godjerry228.github.io/coinvert/
2.  點擊右上角的「設定 (齒輪)」圖示。
3.  點擊 **「加入主畫面」** 選項 (若瀏覽器支援，按鈕會自動顯示)。

---

## 🛠 技術棧 (Tech Stack)

本專案堅持零依賴 (Zero Dependency)，純手工打造高效能體驗：

* **Core**: HTML5, CSS3 (Flexbox/Grid), Vanilla JavaScript (ES6+)
* **Storage**: LocalStorage (保存用戶設定與排序)
* **PWA**: Service Worker (`sw.js`), Web App Manifest (`manifest.json`)
* **API**: [ExchangeRate-API](https://www.exchangerate-api.com/)
* **Assets**: [FlagCDN](https://flagcdn.com/)

## 📂 專案結構

為了確保 PWA 功能正常運作，您的專案資料夾應包含以下檔案：

```text
.
├── index.html       # 主程式 (包含 UI、邏輯與樣式)
├── app.png          # App 圖示 (建議 512x512 或 192x192)
├── manifest.json    # PWA 設定檔 (定義名稱、圖示、啟動模式)
├── sw.js            # Service Worker (處理離線快取)
└── README.md        # 專案說明文件
