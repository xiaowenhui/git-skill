使用步骤
---

1. 安装git
2. 设置全局的 name、email
3. 生成本地SSH key
4. github 上添加SSHkey
5. 新建本地仓库
6. github上新建远程仓库
7. 将本地仓库和远程仓库关联起来
8. 第一次提交
9. 后续提交

创建本地仓库
--
1. 新建工作区（文件目录），mkdir
2. 初始化本地仓库，git init


创建远程仓库
--
1. 登录github，创建一个repository


github上添加ssh key



*查看全局用户名和email：*
 
```
git config  user.name 
git config  user.email  
```

git config user.name

$ git config user.email
--

*设置全局用户名和email：*
 
```
git config --global user.name  "用户名"
git config --global user.email  "邮箱"
```


1.查看本地是否存在ssh key
 
  ```
  cd  ~/.ssh
  ls
  ```
2.生成ssh key

  ```
  ssh-keygen -t rsa -C "your_email@example.com"
 ```
3.github上添加公钥内容id_rsa.pub

4.测试ssh key


```
ssh -T git@github.com
```



将本地仓库和远程仓库关联起来
--
1. 生成
2. git remote add origin git@github.com:xiaowenhui/git-test.git
3. **第一次提交，git push -u  origin  master**
4. git push  --set-upstream origin master















