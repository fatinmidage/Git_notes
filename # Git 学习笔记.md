# Git 学习笔记
## Git常用命令
**git config** --global user.name  # 设置全局用户名

**git config** --global user.email # 设置全局邮箱
**git status** # 查看当前状态
**git config user.name** # 查看用户名
**git config user.email** # 查看用户邮箱地址
**git init** # 初始化版本库
**git add** # 添加需要提交的文件
- *git add "文件全名"*
- *git add "文件1全名" "文件2全名"*
- *git add . # 添加所有文件*

**git commit -m "标记信息"** # 提交暂存区的修改至版本库
**git diff** # 查看修改内容(未提交commit的，即暂存区的)
>git diff HEAD -- 文件全名 # 查看特定文件的修改内容

**git log** # 查看历史记录，简洁显示用"--pretty=oneline参数"
**git reflog** # 查看所有的修改历史
**git reset** # 返回至以前的版本
> git reset --hard HEAD~
> git reset --hard HEAD~~
> git reset --hard 12jhk1

**git checkout -- "文件全名"** # 用版本库里的版本替换工作区的版本
**git restore --staged "文件全名"** # 撤销暂存区的文件修改(会保留工作区的修改)

# github相关
**ssh-keygen -t rsa -C "youremail@example.com"**
生成公钥文件，在 **/用户名/.ssh** 下

**git remote add origin *git@github.com:fatinmidage/test.git***
添加origin远程库

**git branch -M main**

**git push -u origin main**
将本地版本库推送至远程库(origin)，只有首次推送需要使用-u