# JMP_JSL
JMP Script Language 是 JMP 自带的脚本语言

------

# Git 使用帮助

**1.克隆仓库到本地**

git clone https://github.com/Conny-Wang/JMP_JSL.git

**2.添加更新的文件**

git add .

**3.提交暂存区到本地仓库中:**

git  commit -m “这里可以写备注”

参数设置修改文件后不需要执行 git add 命令，直接来提交

 git commit -a -m  "这里写备注"

**4.设置提交代码时的用户信息**

git config --global user.name 'Conny'

git config --global user.email conny@conny.wang

**5.推送代码到远程仓库**

git push

强制推送

git push -f origin main

**6.创建一个标签**

git tag v1.0.0

找到历史提交 commit id

git log --pretty=oneline --abbrev-commit

git  tag v0.9 471fd27

创建带有说明的标签，用`-a`指定标签名，`-m`指定说明文字

git tag -a v0.1 -m "version 0.1 released push url" d5a65e9

推送 tag 到远程仓库 push 单个 tag，命令格式为：

git push origin tag_20170908

push所有tag，命令格式为：

git push --tags

**7.版本回退（将主干分支回退到某个版本）**

git reset --hard d5a65e

回到上一个版本

git  reset  --hard HEAD

 回到回退前版本

git reset --hard aaff087

