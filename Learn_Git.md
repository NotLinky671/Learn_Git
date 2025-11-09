# Learn_Git
## 初始化本地仓库
```bash
git init
```
## 添加文件
```bash
git add *
```
## 提交
```bash
git commit -m "写你做了什么"
```
## 连接 Github 远程仓库
```bash
git remote add origin https://github.com/username/YourProject.git
```
## 推送到 Github
```bash
git push -u origin main
```
`-u` 的作用是：

> **让本地分支与远程分支建立“追踪关系”（tracking relationship）。**

这样做的好处是：以后你只需要输入 git push 或 git pull，Git 就会自动知道要推送/拉取到哪个远程分支。

## 拉取远程内容
```bash
git pull origin main --rebase
```
`git pull`
> **拉取并且合并(git fetch + git merge)**

`--rebase`的作用是：
> **把本地提交接到远程最新版本的后面，而不是合并。**

### 拉取远程不修改本地
```bash
git fetch
```
> **从远程仓库下载最新的分支和提交信息，但不修改你的本地代码。**

## 切换分支
```bash
git switch 你想切换的分支
```

## 创建分支并切换
```bash
git switch -c dev
```

## 查看本地分支
```bash
git branch
```

## 查看远程分支
```bash
git branch -r
```

## 查看所有分支
```bash
git branch -a
```