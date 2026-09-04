# properties-src　—— 物件一頁式「原稿」

各物件專案把做好的一頁式 **push 到這裡**。這裡只放內容，不放成品。

```
properties-src/           A  原稿（本 repo）      ← 各專案 push
        │
        │  build.py（在 properties-admin）
        ▼
properties/               B  成品・GitHub Pages   ← 只有「主題行銷頁」對話寫入
```

## 各專案要做的

1. 目錄命名 `PropCode`：地名英拼＋關鍵數字，例 `WangTian5483`、`Guanlian766`、`TCIP3464`。
   潛銷案再加 `-` 四碼亂碼，例 `ct1300-e58a`。
   **不要用結尾 `b` 或 `-b`** —— 那是成品端簡版分身保留的。
2. 放一份自足的 `<PropCode>/index.html`：照片 base64 內嵌、外部相依只允許 Google Fonts。
3. 一經上線 **不改名、不刪除、不搬家**（連結已發出去，斷了就是客戶開到 404）。
4. push 到本 repo，然後到「主題行銷頁」對話說一聲「更新 `<PropCode>`」。

## 各專案「不要」做的

- 不要做頁尾「認識專案團隊」區塊 —— 建置時會統一套上，自己做的會被整段換掉
- 不要做簡版分身、不要改公開總覽、不要動 `properties` repo
- 不要連回任何索引或管理頁

## 對外導流只允許這四個

| 用途 | 網址 |
|---|---|
| 關於瑞禾 | `reihe-industrial.github.io/web/` |
| 關於現傑 | `mac2good909777-commits.github.io/about-mac/` |
| 睦聚現傑 | `mac2good909777-commits.github.io/about/`　（**不要用** `mac-chang-hub`） |
| 購廠分析 | `mac2good909777-commits.github.io/service-demo/` |

## 部署

```
cd C:\Users\dell\Documents\Claude-DT\projects\20260904-主題行銷頁\properties-src
git pull --rebase origin main
git add -A
git commit -m "新增/更新 <案名>（<PropCode>）"
git push origin main
```

本 repo **不啟用 GitHub Pages**，成品網址一律在成品站（該站無首頁，連結從台帳取）：
`https://mac2good909777-commits.github.io/properties/<PropCode>/`
