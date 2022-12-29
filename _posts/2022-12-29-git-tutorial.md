# Git学习

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
  
  - 
  
  - 将暂存区的内容提交到本地仓库
    
    ```git
    git commit -m "注释说明文字"
    ```
  
  - 推送本地仓库内容到远程仓库
    
    ```git
    git push [origin]
    ```
    
    
