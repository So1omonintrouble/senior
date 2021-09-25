常用命令:

创建:
`git init`

提交:
`git add 文件名`

`git commit "-m 注释说明"`

舍弃改变:
`git reset HEAD 文件名 (已经add)
git checkout -- 文件名`

查看修改:
在git add之后:
`git status
git diff 文件名`

查看版本:
`git log`
(--pretty=oneline只显示一个)

回退版本:
`git reset --hard HEAD^`
(x个^表示上x个版本，或者是HEAD~x)
(回到未来): `git reset --hard 版本号(写出前几位就可以)`
`git relog`: 查看历史命令

删除:
git rm 文件名
git commit

推送:

`git remote add origin git@github.com:so1omonintrouble/senior.git`
(库) `git push -u origin master`
(以后)`git push origin master`
(删除)`git remote rm 库名(origin)`
查看远程库库:`git remote -v`

分支管理:
`git checkout -b dev(分支名)`
=`git branch dev` + `git checkout dev`
(checkout 用来切换分支)
合并分支：`git merge dev`(分支名)
删除分支：`git checkout -d dev`(分支名)

switch来切换分支:
`git switch -c dev`

