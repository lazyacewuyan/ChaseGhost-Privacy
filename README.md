# ChaseGhost 隱私權政策部署說明

這個資料夾是 Meta Data Use Checkup 使用的公開隱私權政策頁面。

## 發布前必做

法定姓名及公開聯絡信箱已填入。提交前仍需確認：

1. Meta 組織驗證的中文法定姓名為「莊鎬鴻」，英文拼寫為「JUANG, HAU-HUNG」。
2. `assa25814@gmail.com` 是可正常收信且願意公開顯示的聯絡信箱。
3. 如果 Data Use Checkup 不需要 **User profile**，提交前移除該權限；目前程式只讀取 App-scoped User ID，沒有讀取 Horizon 使用者名稱或大頭貼。

可用下列命令確認沒有遺留佔位文字：

```powershell
rg -n "資料控制者法定姓名|公開聯絡信箱|LEGAL NAME|PUBLIC CONTACT|CONTACT_EMAIL|發布前必須" PrivacyPolicy/index.html
```

命令沒有輸出後才適合提交 Meta 審查。

## GitHub Pages 部署

由於主要遊戲 repository 是私人專案，隱私政策已獨立發布至公開 repository：

- Repository：`https://github.com/lazyacewuyan/ChaseGhost-Privacy`
- 公開政策：`https://lazyacewuyan.github.io/ChaseGhost-Privacy/`

更新本資料夾的政策後，需要把 `PrivacyPolicy` 的內容同步至上述公開 repository 的 `main` 分支。送交 Meta 前，請再以無痕視窗或手機網路確認公開政策網址不需登入即可開啟。
