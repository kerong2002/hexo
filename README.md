# hexo
## hexo manual
## 安裝使用
1. 安裝Git [Official Website](https://gitforwindows.org/)
2. 安裝Node.js [Official Website](https://nodejs.org/en/download)
3. 請在您想要的路徑，比如D:\\kerong 路徑下，開啟資料夾後，右鍵點Git Bash Here
4. 安裝```npm install -g hexo-cli```
5. 安裝```npm install```
6. 註冊好username.github.io的repositories
7. git config --global user.name "yourname"
8. git config --global user.email "youremail"
9. 驗證一下名稱的郵件是否正確
10. git config user.name
11. git config user.email
12. ssh-keygen -t rsa -C "youremail" 創建ssh
13. 從電腦中.ssh資料夾搜尋id_rsa.pub的檔案，用nodepad開啟
14. 把公開鑰匙丟上github SSH keys
15. ```ssh -T git@github.com```驗證
16. 修改_config.yml資料
17.
 ```
deploy:
  type: git
  repo: https://github.com/YourgithubName/YourgithubName.github.io.git
  branch: master
```
18. ```npm install hexo-deployer-git --save``` 需要部屬的工具
19. hexo clean
20. hexo generate
21. hexo deploy

