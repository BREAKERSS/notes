# git使用指南
## 1. 本地新建git仓库
```shell
  git init
```
该命令将建立本地git仓库 并且在目录下新建.git文件夹

## 2. 上传到本地git仓库中
```shell
  git add .   添加所有将修改添加到暂存区 可以替换.以精确指定文件
  git status  查看暂存区状态
  git commit -m "上传的注释" 正式上传到本地git仓库
```

## 3. 将git链接到GitHub
---
### (1) 配置ssh公钥
SSH公钥默认储存在账户的主目录下的 ~/.ssh 目录(windows在user目录下)
其中id_rsa为私钥，id_rsa.pub为公钥
### (2)

## 其他
首次使用配置
```
  git config --global user.name "demo"
  git config --global user.email "demo@aerothief.com"
```  
