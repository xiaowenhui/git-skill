# 分支操作

将master分支合并到本地分支
--
  git  pull  origin master

将dev分支merge到master分支
--
  git checkout master
  git  pull
  git merge dev
 
创建与合并分支
---
1. 查看分支  git  branch
2. 新建分支  git  branch  分知名
3. 切换分支  git  checkout 分知名
4. 新建+切换分支  git  checkout -b  分知名
5. 合并某分支到当前分支  git merge  分支名
6. 删除分支  git branch -d  分知名
