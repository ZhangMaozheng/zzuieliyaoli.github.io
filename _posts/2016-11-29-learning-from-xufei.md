---
layout: post
title:  "听徐飞叔叔讲 RxJS"
date:   2016-11-29
categories: [JavaScript]
---

之前在饿了么听徐飞叔叔讲过（以下简称叔叔）相同的主题，今天在百姓网相比之前略有拓展。之前的资料在这里 [流动的数据——使用 RxJS 构造复杂单页应用的数据逻辑](https://zhuanlan.zhihu.com/p/23305264)。想着也听了这么多了，简单的记一下自己的收获吧。

## 目的

叔叔做这些的目的就在于：在纷杂的变化中谋求不变。前端框架变化很快，通过 `RxJS` 将 `Model` 层、 `View-Model` 层抽离出来。在此基础上，不管是 `React` 、 `Vue` 、 `Angular` ，只负责两件事：

- 负责渲染数据；
- 通过事件触发数据変更。

这样，`View` 所负责的职责被大大削减。不管框架怎么变，主体的业务逻辑不变，只修改 `View` 层，维护起来实在是方便。

## 流

用 `流` 来处理数据，是我听后最大的感受。接触 `流` 这个概念是在 `SICP` 中，读这本书的时候恰逢有业务需要，就总结过一篇文章：[举例说明：JavaScript中数据流动和数值的处理](/2016-07-25/input-value-modify-validate-update.html)。

## 新观点

叔叔提到了很多新观点：

- 组件之间的沟通，其实是通过 `View-Model` 层来中转的，并不是组件直接相互沟通；
- 注意区分 `View-Model` 层和 `Model` 层。

以上。
