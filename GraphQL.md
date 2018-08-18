## 什么是 GraphQL

GraphQL是Facebook在2012年开发的一种数据查询语言，并在2015年对外发布。它提供了不同于REST的服务体系结构的替代方案。允许客户端定义所需数据的结构，并且从服务端返回完全相同的数据结构。它是一个强类型的运行时，它允许客户端指定需要的数据，因此可以防止返回过多的数据

主要的GraphQL客户端包括Apollo Client和Relay。 GraphQL服务器可用于多种语言，包括JavaScript，Python，Ruby，Java，C＃，Scala，Go，Elixir，Erlang，PHP和Clojure等

## 为什么要使用 GraphQL
GraphQL 能够非常漂亮地解决三个重要的问题：

- 为了得到视图所需的数据，需要进行多轮的网络调用：借助 GraphQL，要获取所有的初始化数据，我们仅需一次到服务器的网络调用。要在 REST API 中达到相同的目的，我们需要引入非结构化的参数和条件，这是很难管理和扩展的。

- 客户端对服务端的依赖：借助 GraphQL，客户端会使用一种请求语言，该语言：1）消除了服务器端硬编码数据形式或数量大小的必要性；2）将客户端与服务端解耦。这意味着我们能够独立于服务器端维护和改善客户端。

- 糟糕的前端开发体验：借助 GraphQL，开发人员只需使用一种声明式的语言表达用户的界面数据需求即可。他们所描述的是需要什么数据，而不是如何得到这些数据。在 GraphQL 中，UI 所需的数据以及开发人员描述数据的方式之间存在紧密的联系。


## GraphQL的设计原则

- **层次分明**：今时今日的大部分产品开发都涉及到创建和操作视图层次。为了满足应用结构的层次性，每个GraphQL查询也是层次构建的，每个查询和其数据共用了相同的形状，这样的方式在描述数据需求上更为直观。
- **以产品为中心**：不可置辩的说，GraphQL是一种视图需求驱动的语言，因为主要是前端工程师书写它。GraphQL从前端工程师的思想和需求出发，再开发了语言和运行时库以满足这些需求。
- **强类型**：每个GraphQL服务器都会构建一个针对应用的类型系统，查询语句就在这个类型系统上下文中执行。对于一个查询语句，GraphQL工具可以在执行以前通过类型系统检查这个查询语句的语法正确性和查询有效性，譬如在开发期，服务器就能保证返回值的形状和特性。
- **客户端定制**：通过类型系统，GraphQL向客户端通告了自己那些可以被消费的能力。而客户端则专注于如何消费这些能力，其查询语句的粒度是字段级的。在大多数没有GraphQL的CS模型应用中，不同的服务端用不同的脚本和入口决定了返回的数据。而GraphQL查询则会返回客户端要求的数据，不多不少。
- **内省**：GraphQL是内省的，一个GraphQL服务器的类型系统必须能用GraphQL语言自身来查询，本规范将后文描述此特性。GraphQL的内省特性使之能成为建造通用工具和客户端库的强大平台。

## 如何使用 GraphQL

## GraphQL VS REST

![](C:\Users\sz08\Pictures\1_fKhxPG5PQ55kDika_UVukw.png)



####   参考链接：

- https://graphql.js.cool/learn/
- http://spec.graphql.cn/
- https://www.howtographql.com/
- https://dev-blog.apollodata.com/graphql-vs-rest-5d425123e34b
- [解析 GraphQL 的查询语法](https://mp.weixin.qq.com/s/nim-KSqO3n2d2qwbTHKBJA)
- [REST将会过时，而GraphQL则会长存](https://mp.weixin.qq.com/s/F55uPAKLI1c78ccsK23ubw)
- [GraphQL 在微服务架构中的实践](https://mp.weixin.qq.com/s/sU8PPwFhM0IcVBB2GJF8Kw)
- [GraphQL 聚合层解放前后端](https://mp.weixin.qq.com/s/kjrMnj9A404RjYtynBqxLw)
