---
layout: post
title:  "Goland 报错 cannot use xx (type string) as the type any"
date:   2022-07-21 22:00:00 +0800
categories: golang
---

## 问题

升级 go 1.18 后，goland 出现了一些奇怪的报错。比如在`panic("implement me")`下出现了红色波浪线。

即报错`cannot use "implement me" (type string) as the type any`。我心想，这么个语法还能报错？我这程序明明能跑，是不是你 goland 坏了。

## 办法
搜了搜，果然[有人问过了](https://youtrack.jetbrains.com/issue/GO-12171)，goland 版本问题，升级到 2021.3.3 以上就可以解决。


## 瞎扯
看起来是 1.18 引入的特性比较多，goland 费了一番功夫才适配好。想起上个月底收到了 [jetbrain 涨价](https://blog.jetbrains.com/blog/2022/06/29/increased-subscription-pricing-for-ides-net-tools-and-the-all-products-pack/)的邮件，又去看了看价格单，全家桶一年会贵一百好几，原价 DDL 是今年 10 月，我可以再犹豫两个月决定续不续费，续单个软件还是续全家桶。

平时订阅了一些技术公众号，golang 有点风吹草动都报团更文。什么出新特性啦，最近写 go 的某大佬离开 google 啦...... jetbrain 涨价竟然没看到有博主推，明明身边 10 个 golang 程序员 9 个在用 goland。或许因为用盗版比例太高了吧，或者大厂程序员都是靠公司付钱自己不关心。

jetbrain 的涨价通知写得蛮真诚的，说 7 年了第一次涨价，此前新增了很多特性都没涨价，对老用户的折扣也一直很大，实在是成本上升到了要涨价的时刻了，以后争取尽量不涨。

不知道这个涨价，能不能算作「我受到了欧美通货膨胀波及」的例子。

Anyway，希望认真做软件的人能挣到钱。

