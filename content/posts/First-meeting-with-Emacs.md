---
title: 和 Emacs 的第一次见面
date: 2020-02-26T20:33:41+08:00
tags: ["Emacs"]
---

## 技术之外

在讨论 Emacs 之前，我先谈论一些技术之外的东西。编程是我最近这几个月慢慢探索，才最终确定的方向。以后的时间还很长，我和它的相处不会太和谐。很多人害怕把自己的弱势一面展现给别人看，觉得别人会因此轻视自己。有这种心理很正常，我现在仍抱有这种心理。

但是如果你因为害怕别人的眼光而让自己停步不前，这对你自己来说是一种损失，对别人来说可能什么都不是。最近这段时间，在技术上的折腾让我越来越能体会到，越在意别人的目光，越有可能让自己一事无成。作为一名技术纯菜鸟，这篇文章是我第一次打算写技术文章。

我听过很多别人的说法：写博客分享不光可以总结归纳留着以后再碰到同样问题时拿过来就用，还能够把自己的问题解决过程分享给别人。这样一举两得的事情，我自然是很喜欢做。但是我犹豫了很久都没开始，因为我觉得自己似乎写不了那么清晰明白的技术分享。

很久以后，我才明白我这种想法是非常不对的。因为文章写得好的人，之前也写得不咋滴；技术分享写得不错的人，之前一定写出来很多技术分享了。因为没有人天生是适合做某一件事儿的。不知道你还记不记得我写过的那篇《[如何成为优秀的开发人员](https://gaotianhe.github.io/2020/02/16/%E5%A6%82%E4%BD%95%E6%88%90%E4%B8%BA%E4%BC%98%E7%A7%80%E7%9A%84%E5%BC%80%E5%8F%91%E4%BA%BA%E5%91%98%EF%BC%88%E4%B8%80%EF%BC%89/)》笔记，笔记中记录道：成为优秀开发人员的第一要素是兴趣。

所以，不要一听别人（比如我）说，没有人天生适合做一件事。自己就想：那我只要在一件事情上花足够的时间，我一定能做好。很不幸地告诉你，这种想法很美好，但真正当你做起来的时候，你会发现自己备受煎熬。走到这一步的人，要么是被逼无奈、为生计所迫，要么是太过迷恋于娱乐，在该努力学习的年纪都用来享受生活去了。

所以不要轻易丢掉本属于自己的机会，因为当你从事的工作是你喜欢并且热爱时，你会发现自己是这个世界上最幸福的人。

以下内容属于今天的主题 Emacs，对于技术不感兴趣的同学可以关掉文章了。

## 初识Emacs

### 知道Emacs

我知道Emacs很偶然。我讲一下发现它的过程。我在阅读编程随想的博客，发现其中一篇软件介绍文：讲的是【自由】绘图工具Graphviz的使用。刚看开头时因为没有什么新鲜感，不就是一个绘图工具吗。看到中间吸引我的东西来了，这款软件不是常见的绘图软件，它需要用一种名字叫DOT的语言进行编程。

然而，我昨天对着随想提供的英文文档看了半天也看不懂，索性放弃。再继续看文章，他说Emacs的编辑器有一个功能——所见即所得。就是每次修改完绘图代码，都能够实时看到具体的改动。我对这个起了兴趣，于是我开始谷歌“Emacs”，后来发现Emacs是一个编辑器，它和Vi/Vim编辑器处于并列地位。技术领域的人们经常争论到底是Emacs好用还是Vim。

看到了很多有关Emacs的信息，它是一款可编程的、可定制的高度自由软件，对于新手还算友好至少有中文文档让我读，虽然不一定能够读得懂。

### 下载Emacs

在[这里](http://ftp.gnu.org/gnu/emacs/windows/)有不同的版本可以下，不过你要先在[官网](https://www.gnu.org/s/emacs/)看看，哪一个版本是稳定版。稳定意味着软件的使用过程中的bug已经很少，不会突然崩溃。我下载的是Windows版本，听说最好在Linux上使用Emacs，但是我时间有限，只能先在Windows上折腾一阵子。

下载下来的是一个zip格式文件，解压后打开bin文件夹下的runemacs.exe。这是一个帮助文档，在文档中间有一个Emacs Toturial，点击进去就是一个快速入门指南。

### 学习Emacs

这一次学习的主要内容是快捷键。

| Emacs 快捷键                                                 |
| ------------------------------------------------------------ |
| C-f   向右移动一个字符                               C-b  向左移动一个字符 |
| C-n  移动到下一行                                      C-p  移动到上一行 |
| C-a  移动到行首                                         C-e  移动到行尾 |
| M-a  移动到句首                                         M-e  移动到句尾 |
| M-f  向右移动一个词【对中文是移动到下一个标记符号】          |
| M-b  向左移动一个词【对中文是移动到上一个标点符号】          |

这些快捷键都是组合键，“C”代表ctrl，“M”在windows上就代表alt。

对于f、b、n、p，它们分别是forward（前进）、backward（回退）、next（下一行）、previous（上一行）。

我不知道a代表什么，e大概是ending吧。

这就是今天的学习内容。