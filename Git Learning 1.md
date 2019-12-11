# git



git init 会初始化文件夹，该文件夹中会出现一个.git的隐藏文件夹

git status 可以查看当前的文件追踪情况：

* 如果文件显示是红色，表示文件并不是在被追踪的状态下
* 如果文件显示是绿色，表示文件处于被追踪的状态下

+++

git文件的4中状态

1. untracked
2. ​	未被追踪的
3. modified      表示工作区修改了某个文件但是没有添加到暂存区
4. staged          表示把工作区中修改的文件添加到了暂存区
5. commited    表示数据被安全地存储在本地库中

git的3层结构：

1. working directory	工作区
2. staging index      暂存区
3. git directory(respository)   版本库

+++

git add 命令是将文件从工作区添加到暂存区

git commit -m "committed note" 命令是将暂存区的文件提交到本地库中

git log 可以查看上一次提交的信息

git add . 可以将本地的所有的文件添加到暂存区

git commit -am "file"  一次性将工作区中的文件全部提交到暂存区中

+++

git的撤销操作

git commit --amend             撤销上一次提交，并将暂存区的文件重新提交

git checkout  -- filename 	如果想要撤销工作区中文件的修改可以使用该命令，会将工作区中的文件												回滚到上一次commit的状态

git checkout -- .   				  可以将工作区中的所有文件回滚到上一次commit的版本

git reset HEAD filename      拉取最近一次提交到版本库中的文件到暂存区，该操作不影响工作区

+++

