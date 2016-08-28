title: Git 大法
speaker: 张屈
url: https://github.com/joneyphair 
transition: vertical3d
files: 
theme: blue 
highlightStyle: monokai_sublime 
headFiles: 
usemathjax: 
date: 2016年08月25日


[slide]

# Git 大法 
---

@张屈


[slide]

# 工作流程
### 你的本地仓库由 git 维护的三棵“树”组成。第一个是你的`` 工作目录``，它持有实际文件；第二个是 ``暂存区``（Index），它像个缓存区域，临时保存你的改动；最后是 ``HEAD``，它指向你最后一次提交的结果。
----------
![](http://rogerdudler.github.io/git-guide/img/trees.png)

[slide]

# 仓库
---

## 创建新仓库
---

``` git init ```
## 将本地仓库和远端仓库关联起来

```git remote add origin git@github.com:joneyphair/demo.git```

## 检出仓库

``` git clone git@github.com:joneyphair/demo.git ```




[slide]

# 分支
---

## 创建dev分支，然后切换到dev分支

``` git checkout -b dev ```

同

``` git branch dev ```
```git checkout dev ```

## 查看本地分支

``` git branch ```

## 删除

``` git branch -D dev ```




[slide]

# 添加
---

``` git add <filename> ```
---

``` git commit  -m "注释信息"  ```
---

<br>

![](/images/git-commit.jpg)


[slide]
# 比对 

``` git diff demo.html ```

<br>

![](/images/git-diff.jpg)


[slide]

# 撤销 
---

### 丢弃工作区的修改

``` git checkout <filename> ```
---

<br>

![](/images/git-diff.jpg)

[slide]
# 回退

``` git reset --hard HEAD^ ```

---
### 回退到任意commit 节点
---

``` git reset --hard <commit_id> ```

<br>

![](/images/git-reset.jpg)


[slide]

# stash 
---

``` git stash save "取一个名字" ```

<br>

``` git stash list ```

<br>

![](/images/git-stash-list.jpg)

<br>

``` git stash pop ```

<br>

![](/images/git-stash-pop.jpg)
[slide]
# 状态 

``` git status ```

<br>

![](/images/git-status.jpg)

<br>

![](/images/git-status-2.jpg)

<br>

![](/images/git-status-3.jpg)

[slide]

# 提交 
### 提交分支到远端仓库
---

``` git push -u origin master ```

## 关联

``` git push --set-upstream origin master ```


<br>

![](/images/git-push.jpg)


[slide]

# 更新 
### 拉取并合并代码
---

``` git pull ```

## 关联

``` git push --set-upstream origin master ```


<br>
![](/images/git-pull.jpg)

[slide]

# 合并 

``` git merge dev ```

<br>

![](/images/git-merge.jpg)
![](/images/git-merge-2.jpg)
![](/images/git-merge-3.jpg)

[slide]
# 历史记录

`` git log ``

---

![](/images/git-log.jpg)

[slide]
# 命令记录

`` git reflog ``
---

![](/images/git-reflog.jpg)


[slide]

#commit规范 

![](/images/commit.jpg)
![](/images/commit-2.jpg)

[slide]

# 结束
### @张屈 一下,马上解决
