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

專案已包含 `.github/workflows/privacy-policy-pages.yml`。將變更推送至 GitHub 的 `main` 或 `master` 分支後：

1. 開啟 GitHub repository 的 **Settings → Pages**。
2. 在 **Build and deployment → Source** 選擇 **GitHub Actions**。
3. 到 **Actions** 查看 `Deploy ChaseGhost privacy policy` 是否成功。
4. 頁面網址通常為 `https://lazyacewuyan.github.io/MR_GhostChase/`。
5. 使用無痕視窗及手機網路測試網址，確認不需登入即可開啟，再貼到 Meta 的「隱私政策網址」。

如果 repository 是 private，請確認目前 GitHub 方案允許 private repository 使用 Pages，或改用公開 repository／其他 HTTPS 靜態網站服務。
