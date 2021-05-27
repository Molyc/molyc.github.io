---
title: Hello World
---
网站使用了hexo-Anatole-Core搭建，介绍搭建过程中出现的问题，发送文章的命令行和一些文档链接。

## 快速开始

Run server、Generate static files、Deploy to remote sites
hexo的三个阶段，运行服务、生成静态文件，更新远程站点。

``` bash
$ hexo new "My New Post"
$ hexo server
$ hexo generate
$ hexo deploy
```

点击 [documentation](https://hexo.io/docs/) 可以得到hexo的更多信息. 如果在使用hexo的时候出现了一些问题, 可以点击这个链接[troubleshooting](https://hexo.io/docs/troubleshooting.html) 找到答案，或者可以在 [GitHub](https://github.com/hexojs/hexo/issues)提问.

## 搭建过程中的问题

1. 出现 Failed at the ejs@2.7.4 postinstall script. 的报错。

   搜索网上的解决方案，大部分表明需要升级node.js的版本，然后给了一串指令，但是在windows环境下，升级node.js的方法只有是在[node官网](https://nodejs.org/en/) 下载最新的安装包，覆盖掉原来的目录版本。

2. 各种版本问题

   在安装各种依赖包之间，先更新npm和cnpm，指令如下：
   
   ```
   npm install -g npm
   npm -g i cnpm
   查看版本：
   npm -v
   cnpm -v
   ```
   
3. 安装相关依赖时，尽量使用`cnpm`, 如 `hexo-renderer-pug`
