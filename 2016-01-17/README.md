# Scala Meetup @ Beijing #1

时间：2016.01.17 周日 14:00 - 17:00

地点：北京市海淀区中关村善缘街 1 号立方庭大厦 1 楼科苑星空咖啡厅

地图：（http://j.map.baidu.com/51mg8）

组织者：[@Hawstein](https://github.com/Hawstein)

参与者：[@Hawstein](https://github.com/Hawstein)，[@hepin1989](https://github.com/hepin1989)，待完善

归结：[@Hawstein](https://github.com/Hawstein)，[@hepin1989](https://github.com/hepin1989)

-----
## 引子

[@Hawstein](https://github.com/Hawstein) 在毕业后加入了豌豆荚，豌豆荚是一家技术氛围非常浓厚和开放的公司，工作后他兴趣转向了 Scala（如下），此后他又建立了 [ScalaChina](http://scalachina.org/) 社区，以推动 Scala 在中国社区的传播和发展，期间也得到了 @dcaoyuan 以及 @hongjiang 的鼓励和支持。再到后来他又建立了 ScalaChina QQ 群，以进一步的方便交流。再一次和群友的聊天过程中，其提出可能组织一次线下的交流活动是更好的交流形式的构想，这也是了本次 Meetup 的最初的萌芽。后来他制作了一个[宣传页面](待补充)，并有幸由 @xring 小范围扩散，后来继而被扩散到 `jvm研究群` 也便有了 [ONEAPM]() 的各位实力干将的加入，使得本次 Meetup 人数从几人扩展到了十几人，其将其 CTO 还不辞辛劳，亲临现场对本次圆桌会议表示关切。

本次活动由 [@Hawstein](https://github.com/Hawstein) 的校友所开的 [科苑星空咖啡厅](待添加) 提供场地，他们为这次 Meetup 在二楼专门提供了一个会议室，[@Hawstein](https://github.com/Hawstein) 早早的赶到并布置了现场。大家基本都在预计的时间点到达了预定的地点。

## 主要内容

本次北京地区的 Scala Meetup 组织形式为 10 ~ 20 人的圆桌，一来是时间仓促，二来该活动是第一次办，决定从简开始。实到 12 人，OneAPM 占了将近一半：）

人到齐后 [@Hawstein](https://github.com/Hawstein) 首先对为何组织这次 Meetup 以及为何不得不限制人数，组织为一个圆桌的形式做了简单的说明，并且对本次Meetup的组织形式做了一个简单的介绍。交流形式为：

1. 大家先进行简单的自我介绍。
2. 1）介绍大家是如何接触到 Scala 这门语言的以及。2）在日常工作中对于 Scala 技术栈的应用。

大家先进行了简单的自我介绍后，又按顺序介绍围绕 （1）怎么接触到 Scala 的以及 （2）自己对于 Scala 技术栈的应用展开了交流，期间大伙提问分享，井然有序，热情洋溢。

-----

@hepin1989 首先聊了他是如何接触到 Play 以及 Scala 的和 Akka 的，以及他学习 Scala 的经历，非常曲折，路子非常野，但最后修成了正果，非常令人佩服。为了使用 Play 和看懂 Play 的源代码，学习了 Scala，而后又了解到了 Play 的底层使用的是 Akka，他为了学习 Scala，去看了很多别的语言和工具如 Clojure/Erlang/Elixir和Haskell 等。现在在畅易游做游戏服务端开发，是 Akka 的重度使用者。他介绍了基于 Akka 实现的服务发现以及 Akka Streams 和 kafka 以及 Graylog 结合做实时日志的应用。游戏后端是 Akka 一个非常适合的使用场景，听 @hepin1989 讲，手游的特点就是新游戏上线后的一段时间，会集中涌入大量的新玩家，花钱买买买来玩游戏。这时候对服务端的实时性要求很高，机器也会上得比较多。一小段时间后，玩家对这个游戏就没什么兴趣了，这时只需要少量机器就能应付了。使用 Akka Cluster 动态伸缩，轻松搞定。另外 actor 模式也非常适合来描述玩家/道具等等概念。@hepin1989 对 Netty的了解也比较深入，目前在翻译《Netty in action》。

@xring 还是大四学生，学习能力非常强，现在在 IBM 实习，也已经拿到了 IBM 的 offer。目前他在IBM做一个大型的机器学习的项目。同时IBM的话主要是在使用 Spark 做数据分析，在会议上我们也了解到IBM非常看好Scala和Spark的应用。

@有祥 就职于 IBM，是 DB2 领域的高级技术专家，深耕于 DB2 在金融系统的应用，期间其介绍了他使用语言的经历，以及各种语言在他职业生涯中的特殊的场景下的使用，其介绍说他们为了性能用 C/C++ 几乎都用最基本的特性，为了将性能发挥大最大化，Scala 是个人兴趣，期间他评论说：`Scala是他学习过的最难的一门语言`，同时也交流了他对函数式编程语言的看法，以及目前他对 Spray 以及 Play 的应用。期间他分享了他们现在的基于 OSGI 的系统的一些优缺点，以及探讨了如何把 Scala 技术栈应用到对 IBM 现有的技术服务栈优化和重构中。

@肖宾 是搞硬件开发出身的，后来机缘巧合在技术交流会上接触到了使用 Scala 技术栈的公司，后来进入该公司做 Scala 开发。

@WillemJiang，Apache Camel commiter，目前就职于 OneAPM，OneAPM 目前也在服务中慢慢开始使用 Scala，他介绍了他最开始接触 Scala 是为了编写 Camel 的 DSL 设计，并且评论说 Scala 在 DSL 设计领域和 Groovy 相比不分伯仲，甚至更优。其将他还趣说了 Groovy 的作者[James Strachan](https://people.apache.org/~jstrachan/)说如果他早先知道 Scala，他就不会搞 Groovy了。也评论了 Typesafe 对于 Scala 的强力推动，以及 @odersky 在 PLR 领域的地位和 Scala 整体的设计。他评论说 Scala 目前借助于 Spark 的确社区日益壮大，但是还是有不少难以逾越的门槛，比如学习曲线太陡，并且形象的描述为`一个快速跑路的人突然遇到一堵高墙`，为此他对于 Scala 中文社区应该如何扩大提出了指导意见以及对 Scala 语言的演进方向做了自己的看法，大家纷纷表示赞同。@WillemJiang 讲了不少 Apache下开源项目相关的事情，比如其在 JBoss、红帽和 Groovy 的作者以及 Trustin 等作为同事一起开发开源项目的工作经历，并且就开源项目的开发、组织以及盈利模式进行了介绍，大家对此也都比较感兴趣，于是大家围绕这个话题聊了一会。另外，@WillemJiang 还对之后的活动形式提了个建议，可以搞一些类似 Hackathon 的活动，让大家用 Scala生态圈中的工具做些好玩的东西。


TODO Detail @cabin 说他很幸运第一次工作边接触到了 Scala 并且正在现在的公司应用并积极推广 Scala。


@张健 OneAPM 讲述了他们目前使用 Scala 来设计 DSL 以及最开始在技术预研是对 Akka 的一些应用。

来参加交流会的 OneAPM 小伙伴还有 @友国，@晓光，@张健，@谢鑫，后来 OneAPM 的 CTO 也到访：）。Scala 在 OneAPM 还不算使用得很多，目前主要用到像 Flink 和 Spark Streaming 做一些流式处理，也有开始使用 Akka。不过看得出来，OneAPM 的小伙伴们对 Scala 充满了热爱，相信 Scala 技术栈会慢慢更多地运用在 OneAPM 的服务中。

最后，[@Hawstein](https://github.com/Hawstein) 对 Scala 在豌豆荚的应用进行了介绍，他引用了他问 @dcaoyuan 为何选择 Scala 时，@dcaoyuan 的回答：`Scala满足了他对编程语言的所有幻想。`，大家纷纷表示惊讶和赞同。而后他分享了其如何使用 Akka Streams 进行实时日志分析，以及评论 Haskell 是最优雅的函数式编程语言。而且也分享了@dcaoyuan 的一些工作，描述说 [Chana](https://github.com/wandoulabs/chana) 是一个大型的实时查询系统的一部分，大家就一些细节问题进行了咨询。同时也分享了 @dcaoyuan 对于 Akka 的高度评价。

> Written by [@Hawstein](https://github.com/Hawstein)
<br>
我个人是函数式编程语言的爱好者，最早接触的是 Haskell，并且深深地被这门语言所吸引。但问题是一直没能用 Haskell 写些实用点的项目，后来在和 @dcaoyuan 的一次聊天中，我的兴趣开始转向 Scala。详见：[我为什么想做 ScalaChina](http://scalachina.org/topic/54fdede715c4020608a15299)。大概有大半年的时间，我工作的时候写 Java，工作之余写 Scala，这种状况在一次公司的结构调整后发生了改变。我和公司另一位偏爱 Scala 的后端工程师开始为一条新产品线写后端服务，这样我也就开始在工作中使用 Scala 了，主项目用到了 Akka，Spray 和 Slick，其它的工具我也都想尝试，于是用 Play 写后台来满足一些后台需求，用 Akka Streams 写日志分析服务来对线上服务的日志进行实时分析处理。使用 Scala 至今，虽然知道它的各种不足，也踩过很多坑，但目前它还是我最喜欢的编程语言。而 Scala 生态圈中，我最喜欢的工具是 Akka，希望后面能用它做些好玩的事情。


在本次会议的最后，大家进行了总结，并且简单地探讨了下次一次可能的形式，并且合照进行了留影纪念。
![cy66tf8wyae0fl9](https://cloud.githubusercontent.com/assets/501740/12428996/dbe3fcd4-bf22-11e5-99ae-b0ca91748598.jpg)

最后在这里再次感谢 [@Hawstein](https://github.com/Hawstein) 组织了这次活动。
