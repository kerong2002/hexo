# Hexo 使用手冊

## 安裝與使用

1. 安裝 [Git](https://git-scm.com/) 和 [Node.js](https://nodejs.org/)
2. 開啟您想要的目錄，例如 `D:\kerong`，右鍵點擊選擇 "Git Bash Here"
3. 在 Git Bash 執行指令 `npm install -g hexo-cli` 安裝 Hexo
4. 在 Git Bash 執行指令 `npm install` 安裝 Hexo 所需的依賴包
5. 在 GitHub 上建立一個新的 repositories，名稱為 `username.github.io`
6. 在 Git Bash 執行指令 `git config --global user.name "yourname"`，設置您的 GitHub 使用者名稱
7. 在 Git Bash 執行指令 `git config --global user.email "youremail"`，設置您的 GitHub 電子郵件地址
8. 驗證使用者名稱和電子郵件地址是否正確：在 Git Bash 執行指令 `git config user.name` 和 `git config user.email`
9. 創建 SSH 金鑰：在 Git Bash 執行指令 `ssh-keygen -t rsa -C "youremail"`
10. 打開電腦中的 `.ssh` 資料夾，找到名為 `id_rsa.pub` 的公開金鑰檔案，用文本編輯器打開
11. 把公開金鑰檔案的內容複製到 GitHub 上的 SSH keys 設置中
12. 在 Git Bash 執行指令 `ssh -T git@github.com` 驗證 SSH 連線是否正確
13. 修改 Hexo 的 `_config.yml` 設定檔案，指定部屬資訊
14. 在 `_config.yml` 中添加以下設定:
 ```yaml
   deploy:
     type: git
     repo: git@github.com:yourname/yourname.github.io.git
     branch: master
 ```
15. 在 Git Bash 執行指令 npm install hexo-deployer-git --save 安裝部屬工具
16. 在 Git Bash 執行指令 hexo clean，清除 Hexo 產生的檔案
17. 在 Git Bash 執行指令 hexo generate，生成靜態網頁
18. 在 Git Bash 執行指令 hexo deploy，部屬網頁到 GitHub 上
### 恭喜您！您的 Hexo 靜態網站已成功部屬到您的 GitHub Pages 上。 
