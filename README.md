# hexo
## hexo manual
## 安裝使用

1. 安裝 Git [Official Website](https://gitforwindows.org/)
2. 安裝 Node.js [Official Website](https://nodejs.org/en/download)
3. 請在您想要的路徑，比如 D:\\kerong 路徑下，開啟資料夾後，右鍵點選 "Git Bash Here"。
4. 安裝 hexo-cli： `npm install -g hexo-cli`
5. 安裝相關套件： `npm install`
6. 註冊好 `username.github.io` 的 repository。
7. 設定 git 使用者名稱： `git config --global user.name "yourname"`
8. 設定 git 使用者信箱： `git config --global user.email "youremail"`
9. 驗證使用者名稱的郵件是否正確： `git config user.name`
10. 驗證使用者信箱是否正確： `git config user.email`
11. 創建 SSH 金鑰： `ssh-keygen -t rsa -C "youremail"`
12. 從電腦中 .ssh 資料夾搜尋 `id_rsa.pub` 的檔案，用 nodepad 開啟。
13. 把公開鑰匙丟上 GitHub SSH keys。
14. 驗證： `ssh -T git@github.com`
15. 修改 `_config.yml` 資料：
```yaml
deploy:
  type: git
  repo: git@github.com:yourname/yourname.github.io.git
  branch: master
```
16. 安裝需要部屬的工具： `npm install hexo-deployer-git --save`
17. 刪除之前生成的網站資料： `hexo clean`
18. 重新生成網站資料： `hexo generate`
19. 部署網站： `hexo deploy`
