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