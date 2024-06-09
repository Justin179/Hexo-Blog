---
title: For my own convenience
date: 2024-05-20
tags:
- 標籤1
- 標籤2
category:
- [主分類1,分類2]
hide: false
top: false
---



## Quick Start

### Local Deployment

1. Modify files locally.
2. Localization testing: ```hexo clean && hexo s.```
3. Deployment: ```hexo g -d.```

<!-- more -->

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Create a new draft

``` bash
$ hexo new draft "My New Draft"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)


### 引用區塊 (Block Quote)

{% blockquote %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque hendrerit lacus ut purus iaculis feugiat. Sed nec tempor elit, quis aliquam neque. Curabitur sed diam eget dolor fermentum semper at eu lorem.
{% endblockquote %}

### 程式碼區塊 (Code Block)

```java
public int pathSum(TreeNode root, int targetSum) {
    hmap = new HashMap<>();
    count = 0;
    dfs(root, 0, targetSum);
    return count;
}
```

單行程式碼`System.out.println("")`


### Code Highlight theme
All available themes: [theme-next.js.org/highlight](https://theme-next.js.org/highlight/)