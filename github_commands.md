# Github Branch 相关操作

## 查看当前远程仓库分支情况，HEAD指针指向

`$ git branch -a`

## 查看本地分支情况

`$ git branch`

## 删除本地分支

`$ git branch -d localBranchName`

## 删除远程仓库分支
`$ git push origin —delete remoteBranchName`

## 创建本地分支

`$ git branch localBranchName`

## 切换分支

`$ git checkout branchName`

## 分支合并

`$ git merge mergedBranchName`

<br>
<br>

# 提交版本撤回，回滚到某次commit

1. `$ git log` 调出日志

![log infomation](./figures/log_info.png)

2. 选择需要回滚的 commit ID，通过reset命令操作, 例如:  

        $ git reset --hard 05ac0bfb2929d9cbwiener75e52ecb011950fb

3. `--hard` 是强制执行的意思，执行上述命令后，再执行如下命令，强推到远程仓库

        $ git push origin HEAD --force






