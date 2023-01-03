---
title:  Git教程
layout: post
categories: git
tags: git
excerpt: git教程
---

_ _ _

# Git学习

## Git仓库初始化

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

+ 提交代码到远程仓库的master分支
  
  ```git
  git push -u orign master
  ```
  
  

## Git指令

- git设置上游仓库并同步
  
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

- git提交
  
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

<img title="" src="file:///C:/Users/Administrator/AppData/Roaming/marktext/images/2022-12-29-17-39-22-1672306758474.png" alt="" data-align="center" width="483">

        显示工作区中有一个文件没有被追踪，使用git add 文件名将该文件保存到暂存区。
