---
id: 63
title: 1.8初步更新完成
date: 2015-02-20T23:38:03+00:00
author: Soniji
layout: post
categories: 
    - categories.announcement
tags:
    - tags.es.name
list-filter: announcement
---
于是现在ES经济生存服需要1.8以上才能进入了~<del>欢迎去找可爱的Guardian玩</del>
  
回归正题，为什么是初步完成？
  
首先，在ES的/warp res仍然是1.7的资源世界，未探索区域会按照1.8区域生成。这个资源世界预计会在22日删除，所以请备份好个人物品~
  
然后目前1.8的新资源世界仍有插件还没安装上去，所以随机传送，前缀，领地等功能都不能正常运作，但是资源采集现在开始已经没有问题了~
  
而全新的1.8资源世界的传送点为`/warp r18`或者`/server rs`，返回主世界时就使用`/server es`之类的就好了

ES是进入服务器时第一个连接的服务器，而现在仅支持1.8进入了。习惯使用1.7的IW空岛生存就无法正确的进入fallback服务器了，于是，现在默认和fallback服务器改为IW直到Lobby服务器的加入。前往ES需要额外使用`/server es`指令了

现在在ES添加了一个新功能，戳聊天栏的名字可以打开用户菜单选择传送之类的功能~
  
但同时这个聊天栏同时存在一些缺字乱码的问题，仍有待修复
  
希望也能在22日前完成这些修复了~

关于能否进行ID更改，目前的答案仍然是不。
  
LWC的数据库还没转换到UUID，所以如果十分确认需要改名字的话，请首先解锁你的容器（使用/cpersist可以批量操作，详情看：<a href="http://wiki.primcraft.com/LWC" target="_blank">PrimCraftWiki的LWC介绍</a>，领地可以寻找管理员修改，日后这两个都应该可以自动支持UUID。而Private Horse暂时没有解决方案。其他插件已能够兼容。