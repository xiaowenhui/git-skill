
git取消文件跟踪
--
1. 在使用git的时候，有些文件是不需要上传的，所以就可以修改   .gitignore

2.果是对所有文件都取消跟踪的话，就是
  git rm -r --cached . 　　//不删除本地文件
  git rm -r --f . 　　//删除本地文件
 
3.对某个文件取消跟踪
   git rm --cached readme1.txt    删除readme1.txt的跟踪，并保留在本地。
   git rm --f readme1.txt         删除readme1.txt的跟踪，并且删除本地文件。

4.然后git commit 即可。但是git status查看状态时还是会列出来
可以通过 .gitignore文件来达到目的
在git init 的目录下建立.gitignore文件，git官方提供的有 该文件，可以加以修改使用
