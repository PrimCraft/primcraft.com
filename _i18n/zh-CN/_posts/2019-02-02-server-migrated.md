---
layout: post
title: 服务器已迁移
date: 2019-02-02 17:17 +0000
author: Soniji
categories: 
    - categories.announcement
list-filter: announcement
---

Linode 宣布 Tokyo 1 节点结束运营，于是咱也就得将服务器搬去 Tokyo 2 了（

因为 Tokyo 2 的到中国大陆网络不如 Tokyo 1 ，于是专线回归了（

primcraft.com在中国大陆会自动解析到大阪的中转点（osk.primcraft.com），其余地区会解析到服务器直连地址（tky.primcraft.com）。大阪中转点到中国大陆大部分地区速度都还可以，至少比直连要好很多（
  
除此之外还有一个香港的中转点（hkn.primcraft.com），华南地区连这个可能会快一些（如果使用率低下的话，咱或许会取消掉（
  
从服务器到大阪中转点大概会有9ms延迟，到香港大概会有52ms延迟，如果使用icmp ping来获得延迟信息的话，记得加上这些数值
  
minecraft里面的延迟显示的话是正确的了所以不需要管上面这些延迟计算的东西

如遇到问题可在论坛发帖请求帮助w