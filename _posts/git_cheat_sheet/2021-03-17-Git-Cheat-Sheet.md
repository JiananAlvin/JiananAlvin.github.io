---
title: Git Cheat Sheet
tags: Git
article_header:
  type: cover
---

[source in English](https://www.loginradius.com/blog/engineering/git-commands/)

[source in Chinese](https://www.runoob.com/note/56524)

## Frenquently Used Commands

```
1) git pull 
>>>> Modifying project

2) git add .
3) git commit  -m 'message about the commit'
4) git push -u origin [branch name]
```

 

## Git Cheat Sheet

![img](https://www.runoob.com/wp-content/uploads/2015/02/011500266295799.jpg)

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<tbody>
  <tr>
    <td class="tg-0pky">git init</th>
    <td class="tg-0pky"># 初始化本地git仓库（创建新仓库）</th>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global user.name "xxx"</td>
    <td class="tg-0pky"># 配置用户名</td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global user.email "<a href="mailto:&#120;&#120;&#120;&#64;&#x78;&#120;&#x78;&#46;&#x63;&#x6f;&#x6d;"><span style="color:#905">xxx@xxx.com</span></a>"</td>
    <td class="tg-0pky"># 配置邮件</td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global color.ui true</td>
    <td class="tg-0pky"># git status等命令自动着色</td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global color.status auto</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global color.diff auto</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global color.branch auto</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global color.interactive auto</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git config --global --unset http.proxy</td>
    <td class="tg-0pky"># remove proxy configuration on git</td>
  </tr>
  <tr>
    <td class="tg-0pky">git clone git+ssh://git@192.168.53.168/VT.git</td>
    <td class="tg-0pky"># clone远程仓库</td>
  </tr>
  <tr>
    <td class="tg-0pky">git status</td>
    <td class="tg-0pky"># 查看当前版本状态（是否修改）</td>
  </tr>
  <tr>
    <td class="tg-0pky">git add xyz</td>
    <td class="tg-0pky"># 添加xyz文件至index</td>
  </tr>
  <tr>
    <td class="tg-0pky">git add .</td>
    <td class="tg-0pky"># 增加当前子目录下所有更改过的文件至index</td>
  </tr>
  <tr>
    <td class="tg-0pky">git commit -m 'xxx'</td>
    <td class="tg-0pky"># 提交</td>
  </tr>
  <tr>
    <td class="tg-0pky">git commit --amend -m 'xxx'</td>
    <td class="tg-0pky"># 合并上一次提交（用于反复修改）</td>
  </tr>
  <tr>
    <td class="tg-0pky">git commit -am 'xxx'</td>
    <td class="tg-0pky"># 将add和commit合为一步</td>
  </tr>
  <tr>
    <td class="tg-0pky">git rm xxx</td>
    <td class="tg-0pky"># 删除index中的文件</td>
  </tr>
  <tr>
    <td class="tg-0pky">git rm -r *</td>
    <td class="tg-0pky"># 递归删除</td>
  </tr>
  <tr>
    <td class="tg-0pky">git log</td>
    <td class="tg-0pky"># 显示提交日志</td>
  </tr>
  <tr>
    <td class="tg-0pky">git log -1</td>
    <td class="tg-0pky"># 显示1行日志 -n为n行</td>
  </tr>
  <tr>
    <td class="tg-0pky">git log -5</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git log --stat</td>
    <td class="tg-0pky"># 显示提交日志及相关变动文件</td>
  </tr>
  <tr>
    <td class="tg-0pky">git log -p -m</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git show dfb02e6e4f2f7b573337763e5c0013802e392818</td>
    <td class="tg-0pky"># 显示某个提交的详细内容</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show dfb02</td>
    <td class="tg-0pky"># 可只用commitid的前几位</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show HEAD</td>
    <td class="tg-0pky"># 显示HEAD提交日志</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show HEAD^</td>
    <td class="tg-0pky"># 显示HEAD的父（上一个版本）的提交日志 ^^为上两个版本 ^5为上5个版本</td>
  </tr>
  <tr>
    <td class="tg-0pky">git tag</td>
    <td class="tg-0pky"># 显示已存在的tag</td>
  </tr>
  <tr>
    <td class="tg-0pky">git tag -a v2.0 -m 'xxx'</td>
    <td class="tg-0pky"># 增加v2.0的tag</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show v2.0</td>
    <td class="tg-0pky"># 显示v2.0的日志及详细内容</td>
  </tr>
  <tr>
    <td class="tg-0pky">git log v2.0</td>
    <td class="tg-0pky"># 显示v2.0的日志</td>
  </tr>
  <tr>
    <td class="tg-0pky">git diff</td>
    <td class="tg-0pky"># 显示所有未添加至index的变更</td>
  </tr>
  <tr>
    <td class="tg-0pky">git diff --cached</td>
    <td class="tg-0pky"># 显示所有已添加index但还未commit的变更</td>
  </tr>
  <tr>
    <td class="tg-0pky">git diff HEAD^</td>
    <td class="tg-0pky"># 比较与上一个版本的差异</td>
  </tr>
  <tr>
    <td class="tg-0pky">git diff HEAD -- ./lib</td>
    <td class="tg-0pky"># 比较与HEAD版本lib目录的差异</td>
  </tr>
  <tr>
    <td class="tg-0pky">git diff origin/master..master</td>
    <td class="tg-0pky"># 比较远程分支master上有本地分支master上没有的</td>
  </tr>
  <tr>
    <td class="tg-0pky">git diff origin/master..master --stat</td>
    <td class="tg-0pky"># 只显示差异的文件，不显示具体内容</td>
  </tr>
  <tr>
    <td class="tg-0pky">git remote add origin git+ssh://git@192.168.53.168/VT.git # 增加远程定义（用于push/pull/fetch）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch</td>
    <td class="tg-0pky"># 显示本地分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch --contains 50089</td>
    <td class="tg-0pky"># 显示包含提交50089的分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch -a</td>
    <td class="tg-0pky"># 显示所有分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch -r</td>
    <td class="tg-0pky"># 显示所有原创分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch --merged</td>
    <td class="tg-0pky"># 显示所有已合并到当前分支的分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch --no-merged</td>
    <td class="tg-0pky"># 显示所有未合并到当前分支的分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch -m master master_copy</td>
    <td class="tg-0pky"># 本地分支改名</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout -b master_copy</td>
    <td class="tg-0pky"># 从当前分支创建新分支master_copy并检出</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout -b master master_copy</td>
    <td class="tg-0pky"># 上面的完整版</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout features/performance</td>
    <td class="tg-0pky"># 检出已存在的features/performance分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout --track hotfixes/BJVEP933</td>
    <td class="tg-0pky"># 检出远程分支hotfixes/BJVEP933并创建本地跟踪分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout v2.0</td>
    <td class="tg-0pky"># 检出版本v2.0</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout -b devel origin/develop</td>
    <td class="tg-0pky"># 从远程分支develop创建新本地分支devel并检出</td>
  </tr>
  <tr>
    <td class="tg-0pky">git checkout -- README</td>
    <td class="tg-0pky"># 检出head版本的README文件（可用于修改错误回退）</td>
  </tr>
  <tr>
    <td class="tg-0pky">git merge origin/master</td>
    <td class="tg-0pky"># 合并远程master分支至当前分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git cherry-pick ff44785404a8e</td>
    <td class="tg-0pky"># 合并提交ff44785404a8e的修改</td>
  </tr>
  <tr>
    <td class="tg-0pky">git push origin master</td>
    <td class="tg-0pky"># 将当前分支push到远程master分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git push origin :hotfixes/BJVEP933</td>
    <td class="tg-0pky"># 删除远程仓库的hotfixes/BJVEP933分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git push --tags</td>
    <td class="tg-0pky"># 把所有tag推送到远程仓库</td>
  </tr>
  <tr>
    <td class="tg-0pky">git fetch</td>
    <td class="tg-0pky"># 获取所有远程分支（不更新本地分支，另需merge）</td>
  </tr>
  <tr>
    <td class="tg-0pky">git fetch --prune</td>
    <td class="tg-0pky"># 获取所有原创分支并清除服务器上已删掉的分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git pull origin master</td>
    <td class="tg-0pky"># 获取远程分支master并merge到当前分支</td>
  </tr>
  <tr>
    <td class="tg-0pky">git mv README README2</td>
    <td class="tg-0pky"># 重命名文件README为README2</td>
  </tr>
  <tr>
    <td class="tg-0pky">git reset --hard HEAD</td>
    <td class="tg-0pky"># 将当前版本重置为HEAD（通常用于merge失败回退）</td>
  </tr>
  <tr>
    <td class="tg-0pky">git rebase</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch -d hotfixes/BJVEP933</td>
    <td class="tg-0pky"># 删除分支hotfixes/BJVEP933（本分支修改已合并到其他分支）</td>
  </tr>
  <tr>
    <td class="tg-0pky">git branch -D hotfixes/BJVEP933</td>
    <td class="tg-0pky"># 强制删除分支hotfixes/BJVEP933</td>
  </tr>
  <tr>
    <td class="tg-0pky">git ls-files</td>
    <td class="tg-0pky"># 列出git index包含的文件</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show-branch</td>
    <td class="tg-0pky"># 图示当前分支历史</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show-branch --all</td>
    <td class="tg-0pky"># 图示所有分支历史</td>
  </tr>
  <tr>
    <td class="tg-0pky">git whatchanged</td>
    <td class="tg-0pky"># 显示提交历史对应的文件修改</td>
  </tr>
  <tr>
    <td class="tg-0pky">git revert dfb02e6e4f2f7b573337763e5c0013802e392818</td>
    <td class="tg-0pky"># 撤销提交dfb02e6e4f2f7b573337763e5c0013802e392818</td>
  </tr>
  <tr>
    <td class="tg-0pky">git ls-tree HEAD</td>
    <td class="tg-0pky"># 内部命令：显示某个git对象</td>
  </tr>
  <tr>
    <td class="tg-0pky">git rev-parse v2.0</td>
    <td class="tg-0pky"># 内部命令：显示某个ref对于的SHA1 HASH</td>
  </tr>
  <tr>
    <td class="tg-0pky">git reflog</td>
    <td class="tg-0pky"># 显示所有提交，包括孤立节点</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show HEAD@{5}</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git show master@{yesterday}</td>
    <td class="tg-0pky"># 显示master分支昨天的状态</td>
  </tr>
  <tr>
    <td class="tg-0pky">git log --pretty=format:'%h %s' --graph</td>
    <td class="tg-0pky"># 图示提交日志</td>
  </tr>
  <tr>
    <td class="tg-0pky">git show HEAD~3</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git show -s --pretty=raw 2be7fcb476</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git stash</td>
    <td class="tg-0pky"># 暂存当前修改，将所有至为HEAD状态</td>
  </tr>
  <tr>
    <td class="tg-0pky">git stash list</td>
    <td class="tg-0pky"># 查看所有暂存</td>
  </tr>
  <tr>
    <td class="tg-0pky">git stash show -p stash@{0}</td>
    <td class="tg-0pky"># 参考第一次暂存</td>
  </tr>
  <tr>
    <td class="tg-0pky">git stash apply stash@{0}</td>
    <td class="tg-0pky"># 应用第一次暂存</td>
  </tr>
  <tr>
    <td class="tg-0pky">git grep "delete from"</td>
    <td class="tg-0pky"># 文件中搜索文本“delete from”</td>
  </tr>
  <tr>
    <td class="tg-0pky">git grep -e '#define' --and -e SORT_DIRENT</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git gc</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">git fsck</td>
    <td class="tg-0pky"></td>
  </tr>
</tbody>
</table>