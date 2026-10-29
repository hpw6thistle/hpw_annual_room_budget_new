# 匿名展示靜態包

將 index.html、assets/、.nojekyll 放在網站根目錄。可部署至GitHub Pages；GitHub不會自動解壓ZIP。沿用部署workflow時，替換網站檔案再推送main。

先選館別／角色，在「密碼」欄輸入另附密碼表中的展示值，再按「登入->」。展示身份為hotel1～hotel12、rsvn、finance；各館各有密碼，rsvn與finance各一組。財務可在帳號抽屜修改密碼或隨機產生密碼；修改僅本分頁生效，改finance密碼後重新驗證。rsvn／finance登入後可在工作範圍自由切館；各館身份僅能進入所屬館別，切換身份須重新登入。既有分頁升級保留全部預算與設定，只更新舊預設密碼及工作位置代號。

前端碼可讀、可繞過，只防誤入，不是正式登入或資料隔離。只能用匿名假資料，不用正式密碼、個資或財務資料。

財務可先進「財務初始設定」保存費用及稅額方式；各館／聯訂提交後才能另建財務草稿。新設定預設1–12月手動稅額；自行選用自動模式時，計算欄位仍唯讀。既有保存的設定／版本不追改。提交鎖定不等於主管核准。

2.0.1已移除展示資料重設功能，更新保留既有已儲存資料。

新key為hotel-budget-anonymous-entry-v2，不讀舊key、不匯入舊站。主管核定與實績匯入仍屬後續規劃。此包不能代替正式後端保存。

目前版本2.0.1，下一版2.0.2。

## GitHub Actions部署

首次在 Settings → Pages → Source 選擇 GitHub Actions。每次推送 main 會檢查網站檔案並部署；也可在 Actions 手動 Run workflow。不需提供個人token。

預期網址：https://hpw6thistle.github.io/hpw_annual_room_budget_new/ （首次部署成功後生效）。本儲存庫只有匿名展示靜態檔，沒有正式後端或正式秘密。初碼表另外交付；前端碼可讀可繞過，不提供真正隔離。

本儲存庫未帶入舊Git歷史。新的GitHub提交與部署仍會產生平台紀錄。
