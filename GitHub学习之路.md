# GitHub Desktop

## Clone a repository

之后添加内容

## Add local repository to Git

## Create a new branch from local and remote

## Update some changes

## The solution to a bug come when you are creativing a new function

### stash all changes

对在工作区的项目所作出的修改进行暂存而返回到进行修改前的项目状态。

Git Desktop 仅可以暂存一个commit

Git 命令可以暂存多个更改commits

### directly switch

直接切换分支到所需要的分支

但在工作区所作出的修改将会被带到新的分支

## Some way back to the private step

### discard

直接丢弃对项目文件的修改，舍弃掉工作区修改的文件

#### 适用场景

工作区的修改还未commit

#### Git 命令

```
git restore <file name>(singal file)

git reset --hard(all files)
```

### reset

在集成协作项目当中是不可以去使用。

没有 push 到远端的状况下撤销到所指定的 commit 状态，在多人协作下容易将他人的修改丢失。

#### 适用场景

还原到某个commit的状态，而舍弃掉在此之后所commit的状态

#### Git 命令

```git
git reset <commit ID>
```

### revert

针对以上 reset 的方法。

可以将要撤销的修改以一种重新生成一个 commit 的方法撤销回来。

在多人协作中推荐使用。

#### 适用场景

使用一个新的提交抵消掉某次 commit 的修改

#### Git 命令

```
git revert <commit ID>
```

### amend

直接修改最新一次有问题的 commit 。

#### 适用场景

只能修改最新的一次的 commit 。

#### Git 命令

```
git commit --amend
```

## The Tag