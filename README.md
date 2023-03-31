# hexo
hexo使用手冊
安裝與使用
安裝Git 官方網站
安裝Node.js 官方網站
開啟您想要的目錄，例如 D:\kerong，右鍵點擊選擇 "Git Bash Here"
在 Git Bash 執行指令 npm install -g hexo-cli 安裝 Hexo
在 Git Bash 執行指令 npm install 安裝 Hexo 所需的依賴包
在 GitHub 上建立一個新的 repositories，名稱為 username.github.io
在 Git Bash 執行指令 git config --global user.name "yourname"，設置您的 GitHub 使用者名稱
在 Git Bash 執行指令 git config --global user.email "youremail"，設置您的 GitHub 電子郵件地址
驗證使用者名稱和電子郵件地址是否正確：在 Git Bash 執行指令 git config user.name 和 git config user.email
創建 SSH 金鑰：在 Git Bash 執行指令 ssh-keygen -t rsa -C "youremail"
打開電腦中的 .ssh 資料夾，找到名為 id_rsa.pub 的公開金鑰檔案，用文本編輯器打開
把公開金鑰檔案的內容複製到 GitHub 上的 SSH keys 設置中
在 Git Bash 執行指令 ssh -T git@github.com 驗證 SSH 連線是否正確
修改 Hexo 的 _config.yml 設定檔案，指定部屬資訊
在 _config.yml 中添加以下設定
```yaml
Copy code
deploy:
  type: git
  repo: git@github.com:yourname/yourname.github.io.git
  branch: master
```
在 Git Bash 執行指令 npm install hexo-deployer-git --save 安裝部屬工具
在 Git Bash 執行指令 hexo clean，清除 Hexo 產生的檔案
在 Git Bash 執行指令 hexo generate，生成靜態網頁
在 Git Bash 執行指令 hexo deploy，部屬網頁到 GitHub 上
您的 Hexo 靜態網站已成功部屬到您的 GitHub Pages 上
