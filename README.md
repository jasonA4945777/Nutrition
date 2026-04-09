# 飲食改造計畫 App

四週台灣外食飲食行為改造計畫，支援習慣打勾、每日筆記、日誌回顧。

## 部署方式（Cloudflare Pages）

1. 把這個資料夾推到 GitHub
2. 進 Cloudflare Dashboard → Pages → Create a project → Connect to Git
3. 選這個 repo
4. Build settings 全部留空（靜態網站，不需要 build command）
5. 部署完成後得到 `yourname.pages.dev` 網址

## 檔案結構

```
index.html     # App 主體
_headers       # Cloudflare 安全標頭設定
_redirects     # 所有路徑導向 index.html
README.md      # 這個檔案
```

## 本地使用

直接用瀏覽器開啟 `index.html` 即可，不需要任何伺服器。
所有紀錄存在瀏覽器的 localStorage，不會上傳到任何地方。
