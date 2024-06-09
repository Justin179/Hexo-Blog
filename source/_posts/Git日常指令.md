---
title: Git日常指令
date: 2024-05-23
tags:
- Git
- 
category:
- [技術,Git]
hide: false
top: false
---



對目錄進行git版控 (files still **untracked**)

```shell
git init
```

stage目錄下全部檔案 (files **tracked**)

```shell
git add .
```

commit 所有狀態為stage的檔案 到Local repo

```shell
git commit -m 'first commit'
```

 

這圖說明了一切<img src="https://raw.githubusercontent.com/Justin179/Typora/main/data/git-commands-work.jpeg" style="zoom:80%;" />



#### 有了local repo之後, push local repo to remote repo

```shell
git remote add origin https://github.com/<user>/<repo>.git
git branch -M main
git push -u origin main
```

1. 建立`local repo`跟`remote repo`的連結
2. 分支改名為main
3. `push local main to remote main`

指令在GitHub新增repo後都會給



#### HEAD & checkout

**`HEAD` 是 Git 中一個動態的指標**，<mark>用來表示你目前所在的位置</mark>

`git checkout <sha1>` 用`git checkout` 切到某個`commit`，`HEAD`就會跟到該`commit`

`checkout`可以理解為取出，從`local repo`取出資料到`working directory`

`git checkout -- .` `working directory`的**資料還原**到最新的`commit`(`HEAD`版本)



#### branch name

`master`/`main`/`dev` 都是分支名稱，這些分支名稱都只是標籤，所謂的刪除分支本質上是在刪除標籤 (例如: `git branch -D dev`)，原本的`commit`都還是存在的





補充:

VS Code 讓Git版控變得直覺，細節的指令已經不重要 







