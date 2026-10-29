# 匿名展示靜態包

將 index.html、assets/、.nojekyll 放在網站根目錄。可部署至GitHub Pages；GitHub不會自動解壓ZIP。沿用部署workflow時，替換網站檔案再推送main。

首頁欄位為「密碼」，沒有欄位提示，按「登入->」進入。展示身份為hotel1～hotel12、rsvn、finance；各館各有密碼，rsvn與finance各一組。財務可修改展示密碼，僅目前分頁生效；修改finance密碼後重新驗證。切館／角色仍須登出重驗。既有分頁升級只更新密碼規則，保留預算與設定。

前端碼可讀、可繞過，只防誤入，不是正式登入或資料隔離。只能用匿名假資料，不用正式密碼、個資或財務資料。

財務可先進「財務初始設定」保存費用及稅額方式；各館／聯訂提交後才能另建財務草稿。自動所得稅欄位唯讀，需要時選手動模式。提交鎖定不等於主管核准。

重設會清本分頁所有館別／角色／來源的草稿、已提交與財務版本、模板、展示碼、損益／稅額、房間／停用與工作位置，重建西門兩份草稿及816間；不刪GitHub、正式DB、其他裝置或下載檔案。

新key為hotel-budget-anonymous-entry-v2，不讀舊key、不匯入舊站。主管核定與實績匯入仍屬後續規劃。此包不能代替正式後端保存。

## GitHub Actions部署

首次在 Settings → Pages → Source 選擇 GitHub Actions。每次推送 main 會檢查網站檔案並部署；也可在 Actions 手動 Run workflow。不需提供個人token。

預期網址：https://hpw6thistle.github.io/hpw_annual_room_budget_new/ （首次部署成功後生效）。本儲存庫只有匿名展示靜態檔，沒有正式後端或正式秘密。初碼表另外交付；前端碼可讀可繞過，不提供真正隔離。

本儲存庫未帶入舊Git歷史。新的GitHub提交與部署仍會產生平台紀錄。
