1. **创建新分支**： git branch branchNam
2. **切换分支**： git checkout branchName
3. **本地分支推送到远程仓库上**： git push -u origin branchName
4. **保存本地的改变到本地仓库的暂存区中**： git add fileName / git add .
5. **撤销保存在本地仓库暂存区上的更改**：  git restore —staged fileName
6. **把本地仓库暂存区的更改提交到本地仓库中**： git commit -m ‘Message’(本次提交说明）
7. **把本地仓库提交到远程仓库**： git push -u origin branchName
8. **如果提交到远程仓库的代码需要回退**：
    1. 查看提交的commit号： git reflog
    2. 先把本地仓库的代码回退到前一个版本号： git reset —hard 前一个版本号,  hard 会把本地的更改一起删除， 而soft则是把本地仓库的更改回退到未缓存的状态 hard 慎用！！！！！
    3. 最后强制推送到远程仓库撤销更改： git push origin branchName —force
9. **如果已经暂存到本地仓库后，在回退**： git reflog -> git reset —soft 前一个版本号
10. **删除本地仓库分支**：git branch -d branchName   -D 强制删除
11. **删除远程仓库分支**： git push origin -d branchName
12. **查看远程所有分支**： git branch -a
13. **查看本地分支**： git branch
14. **根据commitID查看提交的具体详情**：git show commitID
15. **本地与远程仓库保持一致拉取代码**： git pull
16. **本地仓库与远程建立连接**: git remote add origin ~~https://github.com/bend/nihao.git~~
17. 向远程仓库提交代码：git push -u origin branchName
***
ps: branchName是你的分支名称