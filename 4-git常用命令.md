#将master分支合并到本地分支
git  pull  origin master

#将dev分支merge到master分支
git checkout master
git  pull
git merge dev
