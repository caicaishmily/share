## 什么是 GraphQL

GraphQL是Facebook在2012年开发的一种数据查询语言，并在2015年对外发布。它提供了不同于REST的服务体系结构的替代方案。允许客户端定义所需数据的结构，并且从服务端返回完全相同的数据结构。它是一个强类型的运行时，它允许客户端指定需要的数据，因此可以防止返回过多的数据

主要的GraphQL客户端包括Apollo Client和Relay。 GraphQL服务器可用于多种语言，包括JavaScript，Python，Ruby，Java，C＃，Scala，Go，Elixir，Erlang，PHP和Clojure等

## 为什么要使用 GraphQL



## GraphQL的设计原则

- **层次分明**：今时今日的大部分产品开发都涉及到创建和操作视图层次。为了满足应用结构的层次性，每个GraphQL查询也是层次构建的，每个查询和其数据共用了相同的形状，这样的方式在描述数据需求上更为直观。
- **以产品为中心**：不可置辩的说，GraphQL是一种视图需求驱动的语言，因为主要是前端工程师书写它。GraphQL从前端工程师的思想和需求出发，再开发了语言和运行时库以满足这些需求。
- **强类型**：每个GraphQL服务器都会构建一个针对应用的类型系统，查询语句就在这个类型系统上下文中执行。对于一个查询语句，GraphQL工具可以在执行以前通过类型系统检查这个查询语句的语法正确性和查询有效性，譬如在开发期，服务器就能保证返回值的形状和特性。
- **客户端定制**：通过类型系统，GraphQL向客户端通告了自己那些可以被消费的能力。而客户端则专注于如何消费这些能力，其查询语句的粒度是字段级的。在大多数没有GraphQL的CS模型应用中，不同的服务端用不同的脚本和入口决定了返回的数据。而GraphQL查询则会返回客户端要求的数据，不多不少。
- **内省**：GraphQL是内省的，一个GraphQL服务器的类型系统必须能用GraphQL语言自身来查询，本规范将后文描述此特性。GraphQL的内省特性使之能成为建造通用工具和客户端库的强大平台。

## 如何使用 GraphQL

## GraphQL VS REST



####   参考链接：

- https://graphql.js.cool/learn/
- http://spec.graphql.cn/
- https://www.howtographql.com/
- https://dev-blog.apollodata.com/graphql-vs-rest-5d425123e34b

