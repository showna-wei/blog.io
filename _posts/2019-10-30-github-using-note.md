---
layout: post
title: 英语背单词心得体会2
date: 2019-10-30
categories: blog
tags: [语言学习,认知]
description: some tips I gets from the study of reciting English words。
---


---
layout: post
title: github使用note
date: 2019-10-30
categories: blog
tags: [github,软件技术]
description: some tips I gets from the study of reciting English words。
---

# 基本理解
网站是一个各种软件包，以及项目管理工具，可以folk别人的代码，创建分支 branch，自己进行修改，pull提交。如果对方同意你的版本，就merge，将你的版本融合进代码里
1.需要注册账号
2.创建自己的库，public或者private，其中public的才能免费生成静态页面，做博客类，即Github Page
## 基本操作：fork/clone/push/pull
[github中fork,clone,push,pull request的简单理解 - cvper's world ! - CSDN博客](https://blog.csdn.net/cvper/article/details/79035664)

## 客户端管理工具 Github Desktop
> Github Desktop :官方工具
> 
只是版本管理功能，clone，或者folk后将库下载到电脑。运行修改需要自己使用IDE进行修改调试。 
如果文件内容变化，可以利用Github Desktop，pull提交到自己库里

## Github Page博客写作：Jekyll编译

Jekyll是是一个简单、可扩展的静态站点生成器，文本内容支持md格式，github page 内部支持jekyll，所以只要通过它建立网站，上传到github库中，然后设定相关setting，即可。
> http://jekyllcn.com/
> 
安装需求：
1. ruby已安装
2. ruby 命令行进去：
> gem install jekyll bundler
3. cd 进入目录创建网站,并构建服务
> jekyll new myblog
> cd myblog
> bundle exec jekyll serve
4. 在浏览器中打开 http://localhost:4000 网址
```
如果把 $ jekyll serve 换成 $ jekyll serve –watch，则功能和jekyll serve相同，但是可以在服务启动的情况下修改内容并且同步更新。简单说就是，不用再次启动服务就可以刷新浏览器看修改过的内容。
```

## 使用已有的博客模板 : cnfeat为例
在public库的网页，setting中，有pages，选项。里面点选。
利用别人已经写好的模版，使用md文件进行添加每日博文
>cnfeat库GitHub网址：https://github.com/cnfeat/blog.io
>相关介绍：[如何搭建一个独立博客——简明Github Pages与Hexo教程 - 简书](https://www.jianshu.com/p/05289a4bc8b2)
### 初始设置
1. 打开github，点击folk，拷贝到自己项目，setting里面更改项目名
2. 打开自己folk后的工程，点clone，客户端自动拷贝到本地
3. 在desktop客户端中打开库repository，右键，打开本地文件夹，
4. 修改cmake文件，改为自己要的域名
> cmake内容:showna.cnfeat.com
5. 修改后，在desktop客户端，changes下方，点commit提交，然后点击右边的pushing，才将修改上传，反映在网页上
6. .在网页上，点击setting，找到GitHub Pages，选择分支和主题，
7. 邮箱收到邮件，访问博客网址，即可。
```
邮件内容：
The page build completed successfully, but returned the following warning for the `master` branch:
Your site's DNS settings are using a custom subdomain, showna.cnfeat.com, that's set up as an A record. We recommend you change this to a CNAME record pointing at showna-wei.github.io
.……
```
> 博客网址:http://showna.cnfeat.com/ 

#### 旧版本的jekyll-site 重新编译

* 执行：bundle exec jekyll serve
* 提示：“Could not locate Gemfile or .bundle/ directory”
* site目录，新建文件“Gemfile”，具体见 [Ruby x Jekyll 本地调试环境搭建](https://szhshp.org/tech/2015/11/14/localjekyllenv.html)
* 执行： Bundle install


 
### 更新操作

更改博客基本信息，见[介绍网址](https://www.jianshu.com/p/05289a4bc8b2)

* 博客名字及作者信息：_config.yml
* 个人介绍页面：about.md
* 代表作页面：milestone.md
* 文章模板：blog.io/_posts/2015-03-02-how-to-write.md

修改了
增加博文：
* 在blog.io文件夹下面新建md文件，前面带固定的prefix
```
---
layout: post
title: 英语背单词心得体会
date: 2019-10-30
categories: blog
tags: [语言学习,认知]
description: some tips I gets from the study of reciting English words。
---

这里是博客正文。
```
> 更改信息后，需要重新编译后，再上传，不然很多信息不更新！！
> ruby 命令行进入目录 ，运行：bundle exec jekyll serve -watch

[jekyll 部署 - 一些有的没的 - CSDN博客](https://blog.csdn.net/uselym/article/details/73608638)


