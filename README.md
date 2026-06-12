# japanshop-admin 後台

這個資料夾是給 GitHub repo `japanshop-admin` 使用的管理後台。

## 要上傳到 GitHub Pages 的檔案

- `index.html`

GitHub Pages 開啟後，後台網址會像：

```text
https://你的GitHub帳號.github.io/japanshop-admin/
```

## 不用上傳到 GitHub 的檔案

- `supabase-setup.sql`

這個檔案是貼到 Supabase 的 SQL Editor 執行用。

## 後台會做什麼

- 登入管理員帳號
- 修改網站文案
- 新增 / 修改 / 刪除商品
- 上傳商品圖片到 Supabase Storage
- 匯入日本商品範例資料

## 重要

目前前台 `japanshop` 仍然是純前台單檔版。後台資料會存進 Supabase，但前台要響應後台更新，還需要把前台也換成 Supabase 連動版。

HTML 裡只能放 Supabase `anon public key`，不要放 `service_role key`。
