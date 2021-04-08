## github ，git学习笔记

1. 创建github账户，id：zhangfan111

2. 安装git bash

3. 设置SSH Key

   > ```shell
   > ssh-keygen -t rsa -C "569312005@qq.com"		按回车键
   > 输入密码：git123456
   > 
   > ```

4. 添加公开密钥

   > 右上角的账户设定按钮，setting里的SSH Keys，添加ssh key

5. 创建仓库

   > Hello-World

6. clone已有仓库

   > - git bash客户端切换到相应目录，如/d/jyhd_workspace/github_test
   > - git clone git@github.com:zhangfan111/Hello-World.git 输入密码clone

7. 提交到仓库

   > - git add XXX.java	git add命令将文件加入暂存区
   > -  git commit 提交
   > - git push，GitHub上的仓库会被更新

8. 常用命令

   - git status 查看仓库的状态
   - git log 查看提交日志 
     - git log --pretty=short更简洁的显示
     - git log 后加目录名或文件名，只显示与该目录，该文件相关的日志
     - git diff 查看更新前后的差别

9. 分支的操作

   - git branch 列出当前所有分支，当前分支前有*号
   - git branch feature-A 创建分支feature-A
   - git checkout feature-A 切换分支
   - git checkout -b feature-A 创建并切换到新分支feature-A
   - git branch -D fix-B 删除本地分支
   - git reset --hard 回溯历史版本
   - git merge 合并分支 (feature-A分支合并到主分支，需先切换到主分支，git merge --no-ff feature-A)
   - git log --graph 以图表形式输出提交日志
   - git reset 回溯历史版本（git reset --hard 目标时间点的哈希值）
   - git reflog查看当前仓库的操作日志
   - git commit --amend 修改提交信息
   - git commit -am “XXX” 是git add和git commit的合并
   - git rebase -i 压缩历史 git rebase -i HEAD~2
   - 
   
10. 主干分支：是特性分支的原点，也是合并的终点。