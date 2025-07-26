# Website-shortcut
# 📁 Website Shortcut 資料夾管理工具

這是一個支援 **PWA**（可加入主畫面） 的捷徑資料夾管理工具。你可以新增多個資料夾，為每個資料夾儲存常用網站捷徑，支援拖曳排序、編輯、刪除，UI 極簡乾淨且支援離線使用。

---

## 🚀 功能特色

- ✅ 新增網站捷徑並分類資料夾
- ✅ 拖曳排序 (使用 Sortable.js)
- ✅ 支援 PWA → 可加入主畫面
- ✅ 全螢幕無網址列（iOS/Android）
- ✅ 離線也可使用（透過 Service Worker）
- ✅ 本地儲存資料（localStorage）
- ✅ 使用自帶 Inter 字型，不怕離線爆字

---

## 🛠️ 使用技術

- HTML5 / CSS3 / JavaScript (Vanilla)
- Sortable.js 拖曳排序
- 自製 Service Worker (sw.js)
- PWA Manifest 設定
- 字型離線快取（Inter-Regular.woff2）

---

## 📦 專案結構

Website-shortcut/
├── public/
│ ├── index.html # 主頁
│ ├── manifest.json # PWA 設定
│ ├── sw.js # 離線快取
│ └── fonts/
│ └── Inter-Regular.woff2 # 自帶字型


---

## 📲 如何部署 (推薦 Vercel，手機也能用)

### 方法一：使用 Vercel App
1. 安裝 [Vercel App for iOS/Android](https://vercel.com/download)
2. 使用 GitHub 登入
3. 建立新專案，從手機上傳 `/public` 資料夾內的檔案
4. 自動部署完成，網址為 `https://your-app-name.vercel.app`

### 方法二：用 GitHub + Vercel 自動部署
1. 建立一個新 GitHub Repository
2. 上傳這個資料夾
3. 到 [vercel.com](https://vercel.com) 串接 GitHub 部署
4. 完成！

---

## ⚠️ 注意事項

- PWA 的主畫面模式下，Google Fonts 會載入失敗 → 所以本專案採用字型 **本地化 (.woff2)** 方式嵌入
- 所有資料皆存於瀏覽器 `localStorage`，更換瀏覽器會遺失資料
- 若要清除資料，可在瀏覽器開發者工具 → Application → LocalStorage → 清除 `shortcutData`

---

## 🧠 未來可拓展

- ☑️ 資料夾排序
- ☑️ 資料夾封面可自訂圖示
- ❌ 同步至雲端（目前為離線 localStorage）

---

📌 製作人：小喵  
💬 若需幫助，請聯繫nicchen0122@gmail.com 
