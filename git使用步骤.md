# git使用指南
## 1. 本地新建git仓库
```shell
  git init
```
该命令将建立本地git仓库 并且在目录下新建.git文件夹
---
## 2. 上传到本地git仓库中
```shell
  git add .   添加所有将修改添加到暂存区 可以替换.以精确指定文件
  git status  查看暂存区状态
  git commit -m "上传的注释" 正式上传到本地git仓库
```
---
## 3. 将git链接到GitHub
### (1) 配置ssh公钥
SSH公钥默认储存在账户的主目录下的 ~/.ssh 目录(windows在user目录下)
其中id_rsa为私钥，id_rsa.pub为公钥
### (2)上传的远程仓库
添加远程仓库
```
  git remote add origin git@github.com:Aerotheif/notes.git
```
首次上传(将本地的master分支推送到origin主机，同时指定origin为默认主机，后面就可以不加任何参数使用git push了。)
```
  git push -u origin master
```
## 4. 分支管理
#### 新建分支hehe!!!
```
  git branch 分支名
```
#### 切换分支
```
  git checkout 分支名
```
#### 推送到指定的远程分支
```
  git push origin <local_branch_name>:<remote_branch_name>
```
#### 删除分支
```
git push origin :分支名 删除远程分支
git branch -d 分支名 删除本地分支
```
## 其他
#### 首次使用配置
```
  git config --global user.name "demo"
  git config --global user.email "demo@aerothief.com"
```
