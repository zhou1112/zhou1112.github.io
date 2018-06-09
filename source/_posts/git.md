---
title: Git
tags: 
 - git
---
鉴于日常工作中对于git命令生疏，特此学习，以记之

<!--more-->

1. git status
命令用于显示工作目录和暂存区的状态。使用此命令能看到那些修改被暂存到了, 哪些没有, 哪些文件没有被Git tracked到。git status不显示已经commit到项目历史中去的信息。
2. git add <file>
命令将文件内容添加到索引(将修改添加到暂存区)。也就是将要提交的文件的信息添加到索引库中。
3. git add . 
命令将所有的修改文件上传到暂缓区。
4. git commit -m'修改记录'
推送修改到本地库中。
5. git pull
服务器上的仓库中代码拉到本地
6. git push 
将本地仓库修改推送到服务器上的仓库中
7. git merge
合并分支

在本地修改代码add 过后没有提交成功，当前修改代码丢失时执行（8，9条命令）

8. git reset --hard HEAD~1
回退到上一个版本
9. git fsck --lost-found
执行该命令

10. git log
查看提交历史

11. git remote add origin 地址
本地库关联远程仓库

12. git stash 
可用来暂存当前正在进行的工作， 比如想pull 最新代码， 又不想加新commit， 或者另外一种情况，为了fix 一个紧急的bug,  先stash, 使返回到自己上一个commit, 改完bug之后再stash pop, 继续原来的工作。

13. git stash pop
释放stash暂存

14. git diff
命令用于显示提交和工作树等之间的更改。此命令比较的是工作目录中当前文件和暂存区域快照之间的差异,也就是修改之后还没有暂存起来的变化内容。

