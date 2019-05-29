---
layout:     post
title:      新手如何快速搭建GitHubPages
subtitle:   第一次搭建个人主页，记录下整个过程，希望对新手有一些帮助
date:       2019-05-26
author:     LY
header-img: img/banner3.jpg
catalog: true
tags:
    - Blog
---

> 作为纯小白新手，真的完全没概念，只能参照很多前人分享的教程文一步一步来。在此特别感谢GitHub上的大神们。
> 也感谢手把手教我的程序猿童鞋们，在我的Friends里有他们博客的链接。（我不会承认开博客只是因为一个赌约... ...)


# 前言
花了大半天，细细摸索了一遍教程文，创建了一个博客账号。但后面的个人配置对我一个新手来说实在是太复杂了，最终在老司机远程指导下，终于把我的个人博客[LY Blog](https://aprilliu6.github.io)搭建出来了。。。

由于实在没什么概念，加上本人比较懒，所以本篇记录文主要借鉴了两位大神的教程，在此先表达下感谢并做下转载说明。有需要的朋友也可以直接查看他们的文章，基本可以掌握搭建方法。

感谢[qiubaiying](http://qiubaiying.github.io)提供的博客模板

[他的博客](http://qiubaiying.top)

感谢（https://knightyun.github.io）

教程1（https://www.jianshu.com/p/e68fba58f75c）

教程2(https://knightyun.github.io/2018/04/01/github-pages-blog#1.1)

下面直接粗暴进入主题。


# 快速开始

### 从注册一个Github账号开始

要使用 GitHub Pages，首先要注册一个[GitHub](https://github.com/)账号，在此之前，我根本不知道github是什么，也没有想过有一天我要用到。。。

创建用户名的时候注意下，之后我们博客的链接名称一般会和用户名保持一致

![](/img/2019052601.jpg)

接着新建一个仓库

![](/img/2019052602.png)

对新建的仓库进行设置，我也不知道仓库是干什么用的，但是这里主要是用于搭建博客使用，所以建议进行设置的时候，项目名称就写用户名一致的。比如我用户名是AprilLiu6，那么我项目名称就直接命名为aprilliu6

![](/img/2019052603.jpg)

到这里账号和仓库就有了，接下来就是在仓库里面装东西，也就是我们个人博客的具体设计，包括支撑博客首页的一些网页文件和配置文件。对于新手来说，自己搭建这些配置是不可能的，所以直接借鉴一个你喜欢的博主的模板是最快捷的方法。

详情接着看下文


### 拉取喜欢的博主的博客模板

我直接选用了教程文作者的博客模板

搜索 `qiubaiying.github.io` 进入[我的仓库](https://github.com/qiubaiying/qiubaiying.github.io)


![](/img/2019052604.jpg)

点击右上角的 **Fork** 将博主的仓库拉倒你自己的账号下

稍等一下，点击刷新，你会看到**Fork**了成功的页面

![](/img/2019052605.png)


### 修改仓库名

点击**settings**进入设置

![](/img/2019052606.jpg)

修改仓库名为 `你的Github账号名.github.io`，然后 Rename

注意：为了避免博客创建好之后打不开，这里的账号名和仓库名要保持一致，也和你的github用户名保持一致。我就试过一次使用了别的名字，打开博客地址直接显示404错误

![](/img/2019052607.jpg)

点击Rename之后，已经成功了一半。

往下拉，在GitHub Pages这里已经可以看到你成功创建的博客链接

![](/img/2019052608.jpg)

这时你在在浏览器中输入 `你的Github账号名.github.io` 例如:`aprilliu6.github.io`

就可以看到你的博客主页了。

例：
![](http://upload-images.jianshu.io/upload_images/2178672-96b5db55df9db422.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

若是出现

![](http://upload-images.jianshu.io/upload_images/2178672-cfd55a22902a9d2c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

则需要 [检查一下你的仓库名是否正确](#Rename)

其实只要在前面的步骤中严格保证名称一致，基本不会出现这个问题。

这里注意两点：
1、最好直接复制GitHub Pages那里显示的你创建成功的链接，复制到浏览器打开，自己手打容易出现错误，我就碰到了博客地址前面是https开头，我自己输入地址的时候打成了http，导致打不开网页的问题。
2、这时候创建好的博客，里面的内容完完全全是你复制的那个博主的，所以接下来我们需要进行一些配置操作，把原博主的个人信息或界面风格改成自己的，一些不需要的东西删除。才能原原本本还原出一个属于我们自己的博客。



### 整个网站结构

接下来我们开始修改博客的内容，把它逐步变成我们自己的博客。

我们修改主要是通过以下红框中的配置文件进行修改

![](/img/2019052609.png)


很复杂看不懂是不是，不要紧，大部分我们直接使用原作者搭建好的就行了，只需要改动其中几个主要的文件

- `_config.yml` 全局配置文件
- `_posts`	放置博客文章的文件夹
- `img`	存放图片的文件夹

在`_config.yml`全局配置文件里面，我们可以修改博客主页的标题、博客名称、头像、简介等等

在`_posts` 里面，我们可以删除掉原作者原来发表的文章，创建我们自己的博客文章

在`img`里面，我们可以将原作者的图片进行筛选保留，然后上传我们自己喜欢的图片进行使用。博客里面所有需要用到的图片，基本都需要上传至这个文件夹里面。

接下来一步步进行配置


### 上传图片

由于我们在进行配置的时候可能会需要一些自己的图片，所以先讲下怎么上传图片

操作很简单

点击`img`

![](/img/2019052613.png)

点击UploadFiles上传你的图片就可以了，注意一下命名规范，方便自己以后使用

![](/img/2019052614.png)

可以先找一些博客的主页图片、头像图片上传备用，后面我们直接在配置文件里面输入`img/图片文件名.jpg` ，就可以直接调用图片


### 修改博客配置

接下来进行正式的配置

首先来到我们自己的仓库，找到`_config.yml`文件,这是网站的全局配置文件。

![](/img/2019052610.jpg)

点击修改

![](/img/2019052611.jpg)

然后编辑`_config.yml`的内容

![](/img/2019052612.jpg)

接下来我们来详细说说以下配置文件的内容，以及我是怎么修改的：

#### 基础设置

```
# Site settings
title: You Blog    				  	#你博客的标题
SEOTitle: 你的博客 | You Blog    	 #显示在浏览器上搜索的时候显示的标题
header-img: img/post-bg-rwd.jpg  	#显示在首页的背景图片
email: You@gmail.com	
description: "You Blog"  			 #网站介绍
keyword: "BY, BY Blog, 柏荧的博客, qiubaiying, 邱柏荧, iOS, Apple, iPhone" #关键词
url: "https://qiubaiying.github.io"          # 这个就是填写你的博客地址
baseurl: ""      # 这个我们不用填写

```
#### 侧边栏

```
# Sidebar settings
sidebar: true                           # 是否开启侧边栏.
sidebar-about-description: "说点装逼的话。。。"
sidebar-avatar:/img/avatar-by.JPG      # 你的个人头像 这里你可以改成你自己在img里面上传的照片
```
#### 社交账号
展示你的其他社交平台

![](http://upload-images.jianshu.io/upload_images/2178672-ec775a22f76e2f40.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

在下面你的社交账号的用户名就可以了，若没有可以直接删除

```
# SNS settings
RSS: false
weibo_username:     username
zhihu_username:     username
github_username:    username
facebook_username:  username
jianshu_username:	jianshu_id
```

上面的基础设置、侧边栏、社交账号，一行一行仔细看，把所有的原作者的信息全部对应改成自己的信息就可以了。

然后下面还有几段看不懂的，但是好像无关个人信息的代码，这些不用管，保留就好了。

再往下看。


#### 评论系统

博客中使用的是 [Disqus](https://disqus.com/) 评论系统

由于需要在 [官网](https://disqus.com/) 注册帐号后才可以使用，所以我直接把这一段，还有下面的Gittalk那一段都给删了

```
# Disqus（https://disqus.com/）
# disqus_username: qiubaiying

# Gitalk
gitalk:
  enable: true    #是否开启Gitalk评论
  clientID: f2c84e7629bb1446c1a4                            #生成的clientID
  clientSecret: ca6d6139d1e1b8c43f8b2e19492ddcac8b322d0d    #生成的clientSecret
  repo: qiubaiying.github.io    #仓库名称
  owner: qiubaiying    #github用户名
  admin: qiubaiying
  distractionFreeMode: true #是否启用类似FB的阴影遮罩
```

#### 网站统计

集成了 [Baidu Analytics](http://tongji.baidu.com/web/welcome/login) 和 [Google Analytics](http://www.google.cn/analytics/)，到各个网站注册拿到track_id替换下面的就可以了

由于这两个东西我也都没有，所以统计这一整段我也是全部删掉了。。。

```
# Analytics settings
# Baidu Analytics
ba_track_id: 83e259f69b37d02a4633a2b7d960139c

# Google Analytics
ga_track_id: 'UA-90855596-1'            # Format: UA-xxxxxx-xx
ga_domain: auto
```

#### 好友

这里我把原作者的链接替换成我自己的好友的博客链接了。

```
friends: [
    {
        title: "简书·BY",
        href: "http://www.jianshu.com/u/e71990ada2fd"
    },{
        title: "Apple",
        href: "https://apple.com"
    },{
        title: "Apple Developer",
        href: "https://developer.apple.com/"
    }
]
```

#### 保存
将网页拉到底部，点击 `Commit changes` 提交保存

![](http://upload-images.jianshu.io/upload_images/2178672-0781006b5d15d149.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

就完成基本的全局配置了，再次进入你的主页，就已经是修改好后的版本了

![](http://upload-images.jianshu.io/upload_images/2178672-a49ee2975d524c93.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

恭喜你，到这里，你的个人博客就基本搭建完成了

# 关于VScode和GitHub Desktop

在写文章之前，教我进行博客配置的远程老司机，给我介绍了两个软件，可以更方便我们进行我们的博客管理

分别是 [VSCode](https://code.visualstudio.com/) 和 [GitHub Desktop](https://desktop.github.com/)

VScode可以帮助我们更加方便的修改博客配置，哈哈，在这个里面我要上传图片都是直接把图片文件拉进去就可以了，超方便的，编辑什么的也很方便

GitHub Desktop则是方便我们发表博客，也可以理解为把我们在VScode里面所做的更改，同步到GitHub Pages网页上。

安装好这两个软件之后，我们就可以正式开始操作写文章啦。

在这里我使用到的方法，是先利用GitHub Desktop把项目文件克隆下来，然后用VScode打开文件进行编辑，在`_posts`文件夹里面新增及编辑博文，然后使用GitHub Desktop同步到我的GitHub Pages上面。


# 使用VScode进行编辑

首先我们需要用GitHub Desktop把我们整个项目文件克隆下来，克隆的方法见下文，我统一写到后面关于GitHub Desktop的介绍里面了。

接着直接把项目文件夹用VScode打开，可以直接拖入。

![](/img/2019052617.png)

可以看到，在VScode里面左边的所有文件目录，和我们在我的仓库里面看到的是完全一样的。所以不仅仅是发表文章，前面我们说到的所有配置都可以在这里进行修改。看你自己觉得怎么样方便了。

接下来我们开始操作。

首先我们把原作者发布的文章文件全部删除，如果你想保留一些作为参考备用也可以部分保留

上文已经说过，我们所有的博文都放在`_posts`文件夹里面

打开`_posts`文件夹，然后把这个目录下的文章逐一delete就可以了


## 创建

接着在 `_posts` 的文件夹里


新建一个md文件

![](/img/2019052616.jpg)

修改成自己的博文名称，为了保持一定的命名规则，方便以后查找，我统一会按 `年-月-日-文章标题.md` 的格式命名

这样就成功新建了一篇文章，接着使用Markdown编辑文章，最后保存即可。

## 格式

再说一遍，每一篇文章文件命名采用的是`2019-05-26-新手如何快速搭建GitHub Pages.md`时间+标题的形式，空格用`-`替换连接。

文件的格式是 `.md` 的 [**MarkDown**](http://sspai.com/25137/) 文件。

我们的博客文章格式采用是 **MarkDown**+ **YAML** 的方式。

[**YAML**](http://www.ruanyifeng.com/blog/2016/07/yaml.html?f=tt) 就是我们配置 `_config`文件用的语言。

[**MarkDown**](http://sspai.com/25137/) 是一种轻量级的「标记语言」，很简单。[花半个小时看一下](http://sspai.com/25137)就能熟练使用了

大概就是这么一个结构。

由于我还没有接触过MarkDown，所以本人是按原作者的格式进行编辑的，接下来还需要学习下MarkDown的基本语法，后面才能写出自己的文章。

接下来看一下我们每一篇博文的开头要怎么修改，先复制下原作者博文开头的写法如下：

```
---
layout:     post   				    # 使用的布局（不需要改）
title:      My First Post 				# 标题 
subtitle:   Hello World, Hello Blog #副标题
date:       2017-02-06 				# 时间
author:     BY 						# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - 生活
---

## Hey
>这是我的第一篇博客。

进入你的博客主页，新的文章将会出现在你的主页上.
```

按上面的格式，把信息都改成自己第一篇博文的信息。


#利用GithHub Desktop管理GitHub仓库

[GithHub Desktop](https://desktop.github.com/) 是 **GithHub** 推出的一款管理GitHub仓库的桌面软件，换句话说就是将你在**Github**上的文件同步到本地电脑上，并将修改后的文件同步到**Github**远程仓库。

终于要讲GitHub desktop了。

##### 登录

点开应用,会弹出**登录**框，

![](http://upload-images.jianshu.io/upload_images/2178672-adb7d6824e471ef5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

输入你的**GitHub**账号和密码进行登录

![](http://upload-images.jianshu.io/upload_images/2178672-2d7c407ebddbb44f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

##### 克隆项目文件

登录后会看到以下界面，直接点击关联项目

![](/img/2019052618.png)

点击相应的项目后，左下角会出现一个克隆项目的按钮

![](/img/2019052619.png)

把我们在仓库里面的项目克隆下来，直接选择桌面作为保存路径，方便我们后面操作。

克隆完成后，我们就可以在桌面找到这个文件夹了。

##### 使用VScode进行编辑

接着，把克隆下来的文件夹，用VScode打开，直接在VScode里面编辑即可。我们所有在VScode里面操作过的修改，只要点击保存，都可以同步到Desktop里面。

##### 同步和发布

当我们在VScode里面完成了博客文章的编辑后，在GitHub Desktop界面能立马看到这些改动操作的记录，接着只需要在GitHub Desktop里面点击Commit to master。

再点击出现的Push origin ，等进度条同步完成，就大功告成了。

这时候登录你的GitHub Pages，就能看到发表的文章了。


#结尾

到这里基本就掌握了自己写博客文章的基本方法了，终于有一种要完工的感觉。

啊，已经晚上11点多了，终于要搭建好了。

登录我的博客主页去瞧瞧先... 


**心满意足！晚安！**

