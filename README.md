# 🍱 午餐救星 (CHiT)

唔使再每日問同學「今日食乜」。一撳就自動搵晒你身邊嘅餐廳，再玩一場「二選一淘汰賽」幫你決定午餐！

## 點玩

1. 開個網頁，撳 **📍 搵附近餐廳**
2. 允許瀏覽器攞你嘅位置（用嚟搵附近餐廳，唔會上傳到任何伺服器）
3. 揀邊幾間係今日想考慮嘅（預設全選，撳一下就剔走）
4. 撳 **⚔️ 開始淘汰賽**，每次喺兩間之間揀一間，淘汰到剩最後一間 = 今日午餐 🎉
5. 直接撳去 Google Maps 導航

## 技術

- 純前端單一 HTML 檔，零依賴、零後端、免費。
- 定位：瀏覽器內建 Geolocation API。
- 餐廳資料：OpenStreetMap **Overpass API**（完全免費、唔使 API key）。

## 部署（GitHub Pages，免費）

1. Repo Settings → Pages → Source 揀 `main` branch、`/ (root)`。
2. 等一兩分鐘，個網址會係 `https://<你個 username>.github.io/CHiT/`。
3. 手機開個網址，加去主畫面就好似 App 咁。

> ⚠️ 注意：定位 (Geolocation) 需要 HTTPS。GitHub Pages 本身就係 HTTPS，所以冇問題。本機測試請用 `localhost`。

## 之後可以加嘅嘢

- 記住你嘅口味偏好同歷史（localStorage）
- 「最近食過」避免重複
- 自訂加入唔喺地圖上嘅餐廳
- 價錢 / 步行時間 / 評分篩選
