# Git命令

git config --global user.email "309859406@qq.com"

git config --global user.name "minggu-han"

git config --global --list



git log

git log --author "minggu-han"



git init

git add .

git commit -m "本次提交描述信息"



git rm 文件名

```mark
删除
```

git mv 文件名1 文件名2

```mark
重命名
```

git mv 文件名1 文件夹[文件名2]

```mark
移动文件
```



git log -p [文件夹]文件名

```mark
查看文件与上次conmit之间的变化
```

git checkout -- [文件夹]文件名

```mark
还原到上次commit
```

git reset HEAD [文件夹]文件名 

```mark
撤销追踪
```

