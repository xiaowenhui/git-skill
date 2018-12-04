#公司有gitlab，还有github，这就需要使用两个git账号，一个用作公司项目，一个用作自己的项目，本地该如何配置呢

#一、安装git，可以使用git-gui，git-bash

#二、配置第一个账号

 1）进入C:\Users\wenhui.xiao\.ssh目录

 2）打开git-bash

 3）配置第一个账号的用户名和邮箱

      git config --global user.name  "你的名称"   

      git config --global user.email  "你的邮箱"   

 4）生成秘钥对，执行以下命令，当前目录下生成id_rsa、id_rsa.pub两个文件

      ssh-keygen -t rsa -C "你的邮箱" 

 5）github上配置公钥

 6）测试账号

     ssh git@github.com

#三、配置第二个账号

 1）进入C:\Users\wenhui.xiao\.ssh目录

 2）打开git-bash

 3）配置第一个账号的用户名和邮箱

      git config --global user.name  "你的名称"   

      git config --global user.email  "你的邮箱"   

 4）生成秘钥对，执行以下命令，

      ssh-keygen -t rsa -C "你的邮箱" ，回车，输入要生成的秘钥文件名

 5）gitlab上配置公钥

 6）测试账号

     ssh   http://git.51caocao.cn

#四、配置config文件

 1）进入C:\Users\wenhui.xiao\.ssh目录

 2）新建文件名为config的文件，内容如下

    Host git.XXX.cn
        HostName git.XXX.cn
        IdentityFile  ~/.ssh/id_rsa
    Host github.com
        HostName github.com
        IdentityFile ~/.ssh/github
