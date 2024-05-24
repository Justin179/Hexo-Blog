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



對目錄進行git版控 (files still untracked)

```shell
$ git init
```

stage目錄下全部檔案 (files tracked)

```shell
$ git add .
```

commit 所有狀態為stage的檔案 到Local repo

```shell
$ git commit -m 'first commit'
```

 

這圖說明了一切 :star::star::star:<img src="https://raw.githubusercontent.com/Justin179/Typora/main/data/git-commands-work.jpeg" style="zoom:80%;" />

補充: `git checkout HEAD` 則是把資料從local repo取出到working directory



