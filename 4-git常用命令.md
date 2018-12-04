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
查看分支：git branch
创建分支：git branch <name>
切换分支：git checkout <name>
创建+切换分支：git checkout -b <name>
合并某分支到当前分支：git merge <name>
删除分支：git branch -d <name>
