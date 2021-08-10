# Git命令

```mark
git config --global user.email "309859406@qq.com"

git config --global user.name "minggu-han"

git config --global --list
```





```mark
git log

git log --author "minggu-han"
```





```mark
git init

git add .

git commit -m "本次提交描述信息"
```





```mark
#删除
git rm 文件名

#重命名
git mv 文件名1 文件名2

#移动文件
git mv 文件名1 文件夹[文件名2]
```





```mark
#查看文件与上次conmit之间的变化
git log -p [文件夹]文件名

#还原到上次commit
git checkout -- [文件夹]文件名

撤销追踪
git reset HEAD [文件夹]文件名 
```





```mark
#列出所有本地分支
git branch

#列出所有远程分支
git branch -r

#新建一个分支，但依然停留在当前分支
git branch [branch-name]

#新建一个分支，并切换到该分支
git checkout -b [branch]

#切换到dev分支上，接着跟远程origin地址上的dev分支关联起来
git checkout -b dev origin/dev

#合并指定分支到当前分支
git merge [branch]

#删除分支
git branch -d [branch-name]

#强制删除分支
git branch -D [branch-name]

#删除远程分支
git push origin --delete [branch-name]
```

```mark
	一般来说，在目录下用git clone git@github.com:xxx/yyy.git，接着要查看本地的当前分支。
	git branch
	你会看到你在master分支下，这个时候往往会用git checkout -b dev origin/dev这个命令。
	它意思是说，切换到dev分支上，接着跟远程的origin地址上的dev分支关联起来，这里要注意origin代表是一个路径，可以用git remote -v查看，说白了，origin/dev有点像是git@github.com:xxx/yyy.git/dev
	
	接着在dev当前分支下进行操作，add/commit后，用git push origin dev，意思是推送当前的dev分支到远程origin地址的dev分支上。
```

