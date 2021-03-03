<!--
 * @Author: zyxm5
 * @Date: 2021-03-03 11:09:55
 * @LastEditors: zyxm5
 * @LastEditTime: 2021-03-03 12:22:34
 * @Description: git常用命令
-->

# gitskills

## git add file

> 将本地文件添加到暂存区 `git add .` 添加所有暂存区修改文件

## git commit [-option]

> 将本地文件提交到本地仓库

-   -m 添加提交信息

## git push [-option/--option] [origin] [remote]

origin:本地仓库
remote:远程仓库

> 将本地仓库的提交推送到远程仓库 `git push origin HEAD`

### option

- origin d/delete 删除远程仓库中的分支 `git push origin -d/--delete `

## git merge [branch]

branch:分支名称

> 合并请求

## git cherry-pick [branch] [commit-hash] [--option]

commit-hash:commit 对应的 hash 值 `git cherry-pick dev c2440f0`

> 挑选分支中的某些 commit 进行合并

-   --continue 继续本次 cherry-pick
-   --abort 中止本次 cherry-pick
-   --skip 跳过本次 cherry-pick

## git branch [-option] [branch/newbranch]

> 分支

### option

-   a 显示所有分支 `git switch -a`
-   d 删除分支 `git switch -d dev`
-   m [curbranch] newbranch 修改分支(默认当前分支)名称(远端分支只能删除重建，没有修改) `git branch -m dev2`

## git switch [-option] [branch]

> 切换分支  `git switch dev`

-   -c 创建新分支并切换 `git switch -c dev`

## git config [-option/--option]

> git配置相关

### option

- l/list 列出所有配置项

- alias.alias 'cmd' 配置命令的别名 `git config alias.ci 'commit'`
