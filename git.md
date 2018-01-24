##### git命令
### 1. Log
* 查看详细log `git log`
* 查看格式化log `git log --pretty=oneline`
### 2. Tag
* 查看所有tag `git tag`
* 当前commit添加简单tag信息 `git tag -a v1.4`
* 指定commit添加tag信息`git tag -a v1.3.0.1 7d6b96bccf8abf92f8c158bdb6a9e3b867641b53`
* 查看某一tag详细信息`git show v1.4`
* 远程提交tag`git push origin v1.3.0.1`
* 一次性提交本地仓库所有tag到远程`git push origin --tags`
* 根据tag检出新的分支`git checkout -b branchname v2.0.0`
### 3. 撤销操作
* commit提交后发现提交不完整，覆盖上次提交`git commit --amend`
* 取消暂存`git reset HEAD <file>`
* 撤消对文件的修改`git checkout -- <file>`
### 4. 分支
* [分支创建与合并参考](https://git-scm.com/book/zh/v2/Git-分支-分支的新建与合并)
* 创建一个新分支`git checkout -b iss53`
* 删除某一分支`git branch -d hotfix`
* 查看分支详细信息`git branch -v`
* 查看哪些分支已经合并到当前分支`git branch --merged`
* 查看所有包含未合并工作的分支`git branch --no-merged`
### 5. 常用命令
* 删除readme1.txt的跟踪，并保留在本地`git rm --cached readme1.txt`
* 删除readme1.txt的跟踪，并且删除本地文件`git rm --f readme1.txt`