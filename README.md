# WHITE
![](https://cdn.jsdelivr.net/gh/fushaolei/img/20200630015134.png)

示例网站：https://sorryfu.top/

## 配置

<details>
  <summary>_config.yml</summary>
  
```yml

# main menu navigation
menu:
  主页: /
  博文: /archives
  友链: /friend
  留言: /message
  说说: /saysay
  开往: https://travellings.now.sh/

site_name: Sorryfu #网站的名称
author: Sorryfu  #文章的默认作者
icon: https://cdn.jsdelivr.net/gh/fushaolei/img/20200524104925.jpg #标签页图标

#自我介绍
intro:
  title: Hi.I'm Sorryfu.


#主页的按钮，默认是不跳转的连接，如有需要可去home.ejs里修改
home:
  Blog: /archives
  Travellings: https://travellings.now.sh/

#联系方式  
#更多图标：https://remixicon.com/
contact:
  Music:
    - https://music.163.com/#/user/home?id=559125633
    - ri-disc-line
  Bilibili:
    - https://space.bilibili.com/286672419
    - ri-bilibili-line
  Email: 
    - mailto:1563250958@qq.com
    - ri-mail-line
  Github:
    - https://github.com/FuShaoLei
    - ri-github-line

#友链
link:
  BlogWe: https://blogwe.com/
  城南破事: https://www.ronce.cc/
  竹青虫の窝: https://1940879828.github.io/
  CtrlCV博客: https://www.hack-er.cn/
  两小无猜: https://www.cnblogs.com/charlottepl/
  策策的小黑屋: https://www.cnblogs.com/occlive/
  Guan FuQing: https://yiki.tech
  阿瑞: https://wenzia.com
  依尘: https://yichen.online
  TMaize Blog: https://blog.tmaize.net/
  猫鱼的小站: http://catfish6.net/


# Valine评论系统
valine:
  open: true # true | false 是否打开，默认false
  appid: HBismw2vU6hg56PslAF2APW1-gzGzoHsz  #Leancloud应用的AppID
  appkey: k41e2BJYdNbojyHuMnKT5LBK  #Leancloud应用的AppKey
  verify: false #验证码
  notify: true #评论回复提醒
  avatar: robohash #评论列表头像样式：''/mm/identicon/monsterid/wavatar/retro/hide
  #头像类型可见： https://valine.js.org/avatar.html
  placeholder: 留下你来过的痕迹~ #评论框占位符

plugins:
  # 代码高亮，想要使用代码高亮，得先把根目录的_config.yml里的highlight的enable置成false
  highlightjs:
    js: https://cdn.jsdelivr.net/gh/highlightjs/cdn-release@9.18.1/build/highlight.min.js
    css: https://cdn.jsdelivr.net/npm/highlight.js@10.1.1/styles/vs2015.css
    # more: https://www.jsdelivr.com/package/npm/highlight.js?path=styles
```


</details>

### Front-matter可选配置

```yml
toc: true #可选 true 或者 false
author: 某某 #默认为主题_config.yml中的作者
comments: true #可选 true 或者 false
```

另外友链页面的话，要新建一个page
然后按如下配置：
```yml
layout: friend
```
(o゜▽゜)o☆ 先写这么多

## CHANGE LOG

### 2020/06/23
- menu项可自适应（缩小到一定程度会变成一个小抽屉）
### 2020/06/24 
- 加入了主页展示页
- 另加一个“博文”page来专门放博客
- 博文页改成按年份来陈列博文
- 归档页改成了分类页，按类别来陈列博文

### 2020/06/25
- 加入了friend page项
- 字体全部改成了`'Century Gothic'`字体
- 美化了blockquote
- 美化了code

### 2020/06/26
- 在首页加入了联系方式图标
- 加入并美化了滚动条
- 暂时美化了标签页（治标不治本）
- 博文可以自定义作者了（在Front-matter里加入author就可以啦，如果不写的话，默认作者为主题默认作者）

### 2020/06/28
- 删减掉主页不必要的东西，现在更加精简了
- 暂时删除了底栏

### 2020/06/29
- 又加入了底栏，不过样式变得简约了（算是吧）

### 2020/07/01
- 把博客哪一个ejs删了，然后把所有内容都放在了归档页（archives），包含着分类的文章和未分类的文章，未分类的文章会归入一个块里，这下变得更加精简了

### 2020/07/06
- 可配置主页的按钮了(￣▽￣)"
- 主页的大字会根据屏幕大小变换啦（还在考虑中）

## REFERENCE
本主题在开发过程中或多或少的借鉴前人的一些作品，

- [Typora的更新文档](http://support.typora.io/)：我见过很多简约的主题，但是没见过如此简约的主题，再配上好看的字体，简直了，那一刻开始我就马上找到了它的源码，并下手开发hexo版的主题
- [TMaize Blog](https://blog.tmaize.net/)：同样也是简约布局，但是它的归档页是分类的，就是分类名后面跟着文章，再加上之前入坑就是因为想要自己弄一个可以分类后跟文章名的主题，所以就用上了
- [群狼动力](https://volf.club/)：travelling的发起者，原模版是html5up上的，这是我首页的启发（其实我就是照搬的，不过没有抄代码嘻嘻嘻）

## CONTACT
- 1563250958@qq.com
