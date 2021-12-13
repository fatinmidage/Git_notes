# Git 学习笔记
## Git常用命令
设置全局用户名

> **git config** --global user.name

设置全局邮箱

> **git config** --global user.email

查看当前状态

> **git status**

查看用户名

> **git config user.name**

查看用户邮箱地址

> **git config user.email**

初始化版本库
> **git init**

添加需要提交的文件
> **git add**
> - *git add* "filename.md"
> - *git add* "filename1.md" "filename2.md"
> - *git add .* # 添加所有文件

提交暂存区的修改至版本库

> *git commit -m "标记信息"**

查看修改内容(未提交commit的，即暂存区的)

>git diff HEAD -- 文件全名 # 查看特定文件的修改内容

查看历史记录，简洁显示用"--pretty=oneline参数"
> **git log**

> **git log --pretty=oneline**

查看所有的修改历史
> **git reflog**

 返回至以前的版本

> **git reset**
- git reset --hard HEAD~
- git reset --hard HEAD~~
- git reset --hard 12jhk1

用版本库里的版本替换工作区的版本
> **git checkout -- "文件全名"**

撤销暂存区的文件修改(会保留工作区的修改)

> **git restore --staged "文件全名"**

# github相关

生成公钥文件，在 **/用户名/.ssh** 下
> **ssh-keygen -t rsa -C "youremail@example.com"**

添加origin远程库
> **git remote add origin *git@github.com:fatinmidage/test.git***


**git branch -M main**

将本地版本库推送至远程库(origin)，只有首次推送需要使用-u
>**git push -u origin main**

