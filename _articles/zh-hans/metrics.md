---
lang: zh-hans
title: 开源衡量标准
description: 通过持续的追踪项目，帮助你作出最佳决策，以让开源项目更成功。
class: metrics
order: 9
image: /assets/images/cards/metrics.png
related:
  - finding
  - best-practices
redirect_from: /zh-cn/metrics/
---

## 为什么要度量这一切？

数据，只有在充满智慧的运用它，才能发挥出其应有的功效。这不，作为一名开源项目的维护者，以可以利用数据来助自己一臂之力。

当获取到很多的信息之后，就可以做很多事，比如：

* 理解用户对一个新功能是怎么反应的
* 搞清楚新用户是从哪里来的
* 鉴别，并且决定是否支持一个跑偏的使用场景或者功能
* 量化你项目的流行程度
* 知道你的项目是怎样被别人使用的
* 通过赞助商或者赞赏挣点小钱

举个例子，[Homebrew](https://github.com/Homebrew/brew/blob/bbed7246bc5c5b7acb8c1d427d10b43e090dfd39/docs/Analytics.md) 就利用谷歌数据分析，来帮助他们对工作进行了优先级的区分：

> Homebrew 是免费的，完全由志愿者在业余时间维护。所以，我们没有资源去做详细的Hemobrew用户调查从而决定如何更好的设计未来的新功能以及对当前的工作分出优先级。匿名的聚合用户数据分析让我们基于用户如何，何地，何时使用Homebrew来优先考虑某些补丁和功能。

流行程度并不能代表一切。每个人都是因为不同的原因参与到开源项目中来，如果你做项目维护者的原因是展示你的工作成果，公开你的代码，或者只是为了好玩，那么度量标准可能对你来说就不是那么的重要。

如果你想对自己的项目有一个深层次的了解，那么请继续阅读下文介绍的分析项目活跃度的方法。

## 探索

在有人能够使用或者回馈你的项目之前，他们得知道是否有这样的项目存在，问问你自己：_人们都在寻找这样项目吗？_

![traffic graph](../../assets/images/metrics/repo_traffic_graphs_tooltip.png)

如果你的项目是托管在GitHub, 你可以[访问](https://help.github.com/articles/about-repository-graphs/#traffic)
获取诸如多少人访问过你的项目，他们从哪里得知的之类的信息。在你的项目主页，点击"Graphs", 然后"Traffic"。在这个页面，你可以看到:

* **总浏览量:** 项目被查看了多少次

* **总独立访问者:** 多少人查看了你项目

* **关联网站:** 访问者从哪里来的。这个数据能帮助你搞清楚哪里可以接触到你的受众和你为推广做出的努力是不是有效的。

* **受欢迎的内容:** 访问者都查看了你项目的那些内容，按照页面访问量和独立访客数。

[GitHub stars](https://help.github.com/articles/about-stars/) 可以提供一个基本的衡量流行度的标准。然而GitHub 点赞数并不和下载量、使用量直接挂钩，但是他可以告诉你有多少人在关注你的项目。

你也许想要[在特定的地方跟踪可发现的内容](https://opensource.com/business/16/6/pirate-metrics): 举个例子，Google PageRank，会跟踪来自你项目网站的流量，或者跟踪来自其他开源项目或者网站的流量。

## 使用情况

人们在这个广袤而且疯狂的我们称之为互联网的地方，竟然找你了你的项目。理想情况下，当他们看到你的项目的时候，他们会情不自禁的做点什么。第二个问题你要问自己的是：_人们在使用你的项目吗？_

如果你使用一个包管理器，比如说npm或者RubyGems.org，来发布你的项目，你就可以跟踪到下载量。

每个包管理工具可能会对下载量有着大同小异的定义，而且下载量并不直接和安装、使用有关，但是它提供了一个基本的比较标准。尝试使用[Libraries.io](https://libraries.io/) 来跟踪很多流行包管理工具的使用数据。

如果你的项目是托管在GitHub上，再一次切换到"Traffic"
页面，你可以用[clone graph](https://github.com/blog/1873-clone-graphs)看看你的项目在一个给定的日期被克隆了多少次，按照独立克隆者的总克隆数排序。

![clone graph](../../assets/images/metrics/clone_graph.png)

如果使用项目的数量低于发现项目的数量的话，那么就有两个问题值得考虑。他们是：

* 你的项目没有成功的转化你的受众，或者
* 你吸引了错误的受众

举个例子，如果你的项目占据了Hacker News的头版头条，你可能会看到一个流量的高峰，但是与此同时，转化率会比较低，因为Hacker News上所有人都看见了你的项目。如果你的Ruby项目是在Ruby研讨会上宣传的，那么，更有可能从目标受众群体中获得较高的转化率。

努力找出你的受众是从哪里来的，然后在你的项目主页寻求他们的反馈，看看是上述两种情况的哪一种。

一旦知道了都是有那些人在使用你的项目的话，接下来就是看看他们会做些什么，他们是否基于源代码开始构建？为项目增加新的特性？他们将项目用于科研？还是业务？

## 留存情况

人们找到了你的项目，而且已经在使用了。那么接下来你要问自己的问题就是：_人们有对这个项目做贡献吗?_

不管什么时候考虑贡献者这个问题都不能算早。没有大众的参与，你就可能会把自己置于一个尴尬的境地，那就是你的项目虽然很 _流行_（很多人用）但是并不被 _支持_（维护者没有足够的时间来满足用户的需求）。

保持项目的进展需要[贡献者的流动](http://blog.abigailcabunoc.com/increasing-developer-engagement-at-mozilla-science-learning-advocacy#contributor-pathways_2)（意思是有进有出）因为之前很活跃的贡献者也可能会去干别的事情。

可能会经常用的衡量社区的指标包括：

* **贡献者的总数和每个贡献者的提交次数：** 有多少贡献者，哪些是活跃的，哪些是不活跃。github上，你可以在"Graphs" -> "Contributors"面板查看这些信息。目前，这个图标只计算了那些往仓库默认分支推送的贡献者。

![contributor graph](../../assets/images/metrics/repo_contributors_specific_graph.png)

* **第一次，偶尔为之的，和持续的贡献者：** 帮助检测是否有新的贡献者，以及他们是不是会再来。（偶尔的贡献者是那些提交的次数很少的人，当然啦，这个数目是多少取决于你，比如说五次。）如果没有新的贡献者，你的项目就会停滞不前。

* **打开的issue的数目和PR的数目：** 如果这些数目太高，就意味着你可能需要有人帮你给issue分类以及做代码审查。

* **所有的打开过的issue和PR：** 一个issue被人提出说明你的项目对他来说比较重要。如果这个数目随着时间在增长，这就意味着人们对你的项目感兴趣。

* **不同种类的贡献者：** 比如说，提交代码，修复笔误或者bug，或者在issue下面评论。

> ![](https://avatars.githubusercontent.com/arfon?s=180)
> 开源远远不止代码，成功的开源项目包括代码、文档，以及它们在演进过程中的所有讨论。
> — @arfon, ["开源的形态"](https://github.com/blog/2195-the-shape-of-open-source)

## 维护者活动情况

最后，你还需要确定一件事，那就是维护者有足够的能力和时间处理社区的贡献。最后一个问题你要问自己的是：_我是不是对社区有足够的时间和精力来响应？_

没有责任心的维护者绝对是开源项目的灾难。想象一下就知道，假如一位贡献者提交了代码或其他贡献，但从来没有得到过维护者的回应，Ta 100% 会感到灰心，并最终选择离开。

[来自Mozilla的研究](https://docs.google.com/presentation/d/1hsJLv1ieSqtXBzd5YZusY-mB8e1VJzaeOmh8Q4VeMio/edit#slide=id.g43d857af8_0177) 说： **维护者的响应是鼓励更多贡献者中非常重要的一环**。

考虑记录一下你或者其他的项目维护者对一次贡献（issue或者PR）响应的时间，响应并不需要花多少精力。哪怕只是说一句："谢谢你的贡献，我下周会查看的。"

你也可以测量一在一个贡献被处理的过程中状态变化的时间。比如：

* 一个issue保持打开状态的时间（也就代表一个问题保持没有被解决状态的时间）。
* 一个issue是否因为一个PR得到了解决。
* 陈旧的issue是否被关闭了（被解决的问题应该关闭）。
* 合并一个PR的时间。

## 通过统计 📊 来了解人们的习惯

理解一些细节能够帮助你建设活跃的、成长的开源项目。哪怕是你无法追踪每一个细节，通过使用上述的框架，将能够让你集中精力到该用力的地方，进而助项目成功！
