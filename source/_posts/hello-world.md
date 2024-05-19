---
title: Hello World
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
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

### Local Deployment

1. Modify files locally.
2. Localization testing: ```hexo clean && hexo s.```
3. Deployment: ```hexo g -d.```

### 引用區塊 (Block Quote)

{% blockquote %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque hendrerit lacus ut purus iaculis feugiat. Sed nec tempor elit, quis aliquam neque. Curabitur sed diam eget dolor fermentum semper at eu lorem.
{% endblockquote %}

### 程式碼區塊 (Code Block)
``` Java
alert('Hello World!');
System.out.println("Hello World");
```

{% codeblock lang:Java %}
alert('Hello World!');
System.out.println("Hello World");
{% endcodeblock %}

{% code lang:Java %}
alert('Hello World!');
System.out.println("Hello World");
{% endcode %}

