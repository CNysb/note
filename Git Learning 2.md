# git 

## github 与本地git的关联

1. 使用ssh

   + ssh-keygen -t rsa -C "email"

   + 需要在本地的.ssh/隐藏文件下使用
   + 创建的ssh是需要使用公钥（文件名中带pub）
   + 通过ssh -T git@github.com 来检查是否连接上ssh

2. 添加远程仓库

   + git remote add origin (ssh)
   + git pull origin master --allow-unrelated-histories
   + git push -u origin master

   

   +++

   **创建一个新的远程仓库并连接到本地**

   1. 创建一个新的空文件夹和新的远程仓库
   2. cd到新的空文件夹，git init
   3. 在新文件夹中创建一个README.md，并且在git中追踪且commit
   4. 关联本地和远程仓库  git remote add origin (ssh)
   5. git push -u origin master

   

+++

**将一个已有的远程仓库关联到本地**

1. git clone (ssh)

2. 在本地创建一个新的文件，commit 并且push

   

