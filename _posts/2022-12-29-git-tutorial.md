---
title:  Git教程
layout: post
categories: git
tags: git
excerpt: git教程
---

_ _ _

# Git学习

## 仓库初始化

+ 先在Github或其他远程仓库网站建立个人仓库

+ 初始化本地仓库
  
  ```git
  git init
  ```

+ 添加本地文件到工作目录
  
  ```git
  git add .
  ```

+ 追踪本地本地到本地仓库
  
  ```git
  git commit -m "初始提交"
  ```

+ 设置远程仓库地址
  
  ```git
  git remote add orign 远程仓库地址
  ```

+ 提交代码到远程仓库的main分支
  
  ```git
  git push -u orign main
  ```

## 分支操作

所有操作在main分支上，已知存在一个master分支

+ 建立一个新的分支main
  
  ```git
  git checkout -b main
  ```

+ 查看当前存在的分支
  
  ```git
  git branch
  ```

+ 合并分支master到分支main
  
  ```git
  git merge master
  ```

+ 提交分支
  
  ```git
  git pull origin main --allow-unrelated-histories
  
  NOTE:
  加上后面这个选项允许不相关历史提交
  --allow-unrelated-histories
  ```

+ 删除本地分支master
  
  ```git
  git branch -D master
  ```

+ 删除远程库上的分支master
  
  ```git
  git push origin --delete master
  ```

## 设置上游仓库并同步

- 添加上游仓库
  
  ```git
  git remote add upstream 远程仓库地址
  ```

- 查看目前远程仓库信息
  
  ```git
  git remote -v
  ```

- 拉取上游仓库到本地
  
  ```git
  git fetch upstream master
  ```

- 合并代码
  
  ```git
  git merge upstream/master
  ```

- 推送到自己的仓库
  
  ```git
  git push [origin]
  ```

## 提交

- 将工作目录内容添加到暂存区
  
  ```git
  git add .
  ```

- 将暂存区的内容提交到本地仓库
  
  ```git
  git commit -m "注释说明文字"
  ```

- 推送本地仓库内容到远程仓库
  
  ```git
  git push [origin]
  ```

- 查看文件或文件夹在工作区和暂存区中的状态
  
  ```git
  git status
  ```

## 常用操作总结
+ 更新代码
```git
git stash 
git pull --rebase
git stash pop 
解决冲突文件
```
+ gerrit上代码还未合并时,更新上次提交
```git
git commit --amend --no-edit
```
+ 回到上次提交
```git
git reflog
git reset commitID（之前的commitID）
```