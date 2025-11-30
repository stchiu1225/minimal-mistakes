---
layout: single
title: "ST Picks 內容匯入狀態"
date: 2025-11-30 00:00:00 +0000
permalink: /stpicks-import-status/
---

目前無法直接從 Facebook 粉絲專頁 <https://www.facebook.com/stpicks/> 取得文章內容，嘗試連線時遭到 403 禁止連線。若後續可以存取，請依下列步驟將文章完整同步至本站：

1. 打開粉絲專頁，逐篇複製貼上文章文字、圖片與影片的說明文字。
2. 每篇文章各自建立一個 Markdown 檔，放在 `docs/_posts/` 目錄，檔名格式為 `YYYY-MM-DD-<slug>.md`。
3. 在檔案開頭加入 Jekyll Front Matter，例如：
   ```yaml
   ---
   layout: single
   title: "貼上 Facebook 貼文標題"
   date: 2025-11-30 12:00:00 +0000
   categories: stpicks
   tags: [facebook, repost]
   ---
   ```
4. 在 Front Matter 下方貼上貼文正文，若有圖片請將檔案加入 `docs/assets/`（或其他既有資產路徑），並使用 Markdown 插入。
5. 重新啟動或重新部署站點以確認文章出現在首頁與分類頁。

> 若仍無法連線至 Facebook，可改由擁有存取權的夥伴手動匯出貼文內容，或使用企業級匯出工具，將匯出的 Markdown／HTML 內容放入上述目錄。
