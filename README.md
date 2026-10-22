# 杏子の存鑽與存歌

可直接部署到 GitHub Pages 的靜態網站，依照參考網站的架構製作，主題改為米黃色非洲菊風，瀏覽器分頁圖示為 🌼。

## Google 試算表

https://docs.google.com/spreadsheets/d/1bwftr2QthC008_3SoUrCADGEFwtyfSeD3avWS5LQj4Y/edit?usp=sharing

- A～E 欄：沿用參考網站的表格顯示方式，預設欄位為「存鑽老闆、存鑽數量、存歌數量、存爆數量、總數」。
- L 欄為設定名稱，M 欄為設定內容；網站會讀取「網站標題」與「網站小標題」設定，修改儲存格後重新整理網站即可看到更新。
- 請確認試算表「共用 → 一般存取權」設定為「知道連結的使用者 → 檢視者」，網站才能讀取資料。
- 預設讀取第一個分頁（gid=0）。若資料位於其他分頁，請在 `script.js` 修改 `SHEET_GID`。
- 網站只會讀取試算表，無法直接從網站編輯試算表儲存格；L/M 欄請直接在 Google Sheets 編輯。

## GitHub Pages 部署

1. 解壓縮 ZIP。
2. 將 ZIP 內所有檔案（不是外層資料夾）上傳到新的 GitHub Repository 根目錄。
3. 開啟 Repository 的 `Settings → Pages`。
4. 選擇 `Deploy from a branch`，分支選 `main`、資料夾選 `/(root)`，再按 `Save`。

## 功能

- 依 A 欄名稱搜尋與「顯示全部」。
- 顯示 A～E 欄資料，數字自動加入千分位。
- 讀取 L/M 欄網站標題與小標題設定。
- 米黃色非洲菊主題、花朵分頁圖示與漂浮裝飾。
- 版權署名維持 `© 2026 LionLionTomato. All Rights Reserved.`
