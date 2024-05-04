win+shift+s：截图



Git使用

## 上传文件

1. 初始化文件为代码仓库：git init

   代码区样子

   <img src="C:\Users\zhao.sir\AppData\Roaming\Typora\typora-user-images\image-20240503155148291.png" alt="image-20240503155148291" style="zoom:80%;" />

2. git add -A 所有文件提交,进入暂存区
3. git commit -m "提交信息" ,将所有文件提交进仓库

## 下载文件

git clone url

## 维护项目日常

1. 未提交的工作区回滚

   git checkout 文件名

2. 提交后撤回，仓库恢复了，再将文件回滚：git checkout 文件名

   git resert HEAD：表示定位到当前的提交

   git reset HEAD^数字

   git reset HEAD^1：表示定位到当前的提交的前一个,删除了当前这个HEAD

   

## 分支：每个分支对应一个仓库，修改后记得提交

1. 以当前分支为基础新建分支

   git checkout -b<branchname>

   一般都以master为主分支，在master下新建分支

   切换主分支：git checkout master

2. 列举所有的分支

   git branch

3. 单纯地切换到某个分支

   git checkout <branchname>

4. 删掉特定的分支

   git branch -D<branchname>

5. 合并分支(在master分支下，合并别人)
   git merge <branchname>

![image-20240503164201705](C:\Users\zhao.sir\AppData\Roaming\Typora\typora-user-images\image-20240503164201705.png)

## Git 与 Github 远程仓库

1. 推送当前分支最新的提交涮远程

   git push

2. 拉取远程分支最新的提交到本地

   git pull

一般是先pull最新的提交，在本地进行修改、解决冲突后，再提交

