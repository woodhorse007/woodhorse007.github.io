---
title: Git使用备忘
date: 2018-06-03 19:56:44
tags:
---
#概念
* origin:是仓库的起点
* master:主干

#同步仓库
* git pull --rebase origin master   %下载并合并
* git fetch origin master  %只下载，不合并 
* git clone git@github.com:whatever/something.git  % clone,并建立本地仓库
git pull = git fetch + git merge
git pull --rebase = git fetch + git rebase
#本地记录版本
* git add *  %增加文件
* git commit -m "log" %本地增加版本记录
#上传仓库
* git push origin master
#查看信息
* git branch -a %显示本地仓库的所有分支：本地的，远程的
* git remote -v %列出当前程序对应的所有远程版本仓库的信息，含仓库名和仓库地址（ v 是verbose 的缩写)
