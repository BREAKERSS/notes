# git使用指南
## 1. 检出项目到本地
```shell
	git clone git@gitee.com:aerothief/GY-mall.git
```
## 2. 提交项目
---
* 查看工作区状态
```shell
	git status
```
* 建立跟踪，全部填写'.'
```shell
	git add [文件名]
```
* 撤销跟踪
```shell
    git rm -r --cached [文件名]
```
* 提交到本地仓库
```shell
    git commit
```
* 连接远程仓库（只需一次）
>origin为远程仓库名，也可以取别的名字

```shell
	git remote add origin git@git.com/xxx/xxx.git
```
* 发布本地提交
	>首次提交加上-u，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。

```shell
	git push [-u]
```
3. 恢复历史版本
* 查看提交日志
```shell
	git log
```
* 恢复历史
```shell
	git reset --hard commit值
```
* 回到未来
```shell
	git reflog
```
4.建立新分支
---
* 从master分支建立新分支，并切换
```shell
	git checkout -b v1.0 origin/master
```
* 推送到远程仓库
```shell
	git push origin HEAD -u
```
