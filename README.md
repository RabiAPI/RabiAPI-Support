
<p align='center'><img width="100" height="100" src="/previews/icon.png"></p>

# RabiAPI - 开箱即用的Java项目接口文档生成工具

<p align='center'><img src="/previews/home.png"></p>

## 下载地址

RabiAPI目前是MacOS平台独占软件，仅在Mac App Store提供购买。

* [Mac App Store](https://apps.apple.com/cn/app/id1524200727)

## 版本更新

* [RELEASE_NOTE](/RELEASE_NOTE.md)

## 使用指南

 - [使用指南](https://github.com/RabiAPI/RabiAPI-Support/wiki)
 - 产品支持QQ群：**244365684**

## 功能特色

**极简的使用方式，零学习成本，零配置，零额外依赖，不需要构建你的项目，不需要运行任何测试方法/Main方法，真正意义上的开箱即用!**

* 通过静态分析解析Java源代码，直接生成文档。
* 支持Java原生接口写法，Spring Boot 注解，Jax-RS 注解。
* 导出文档为Markdown，Asciidoc，PNG图片格式。
* 与Git集成，直接使用分支生成与管理文档。
* 支持泛型类型推导，List，Map展示。
* 多模块项目支持，左侧模块列表中可以切换不同的模块。

## 支持的Java类型和语法

* 所有Java基本类型
* 所有Java容器类型，List、Set、Map
* Java日期时间类型
* 泛型和继承语法，自动推导泛型和继承的结果
* 循环依赖和递归提示
* 内部类支持
* 方法重载支持
* 枚举类型支持展示枚举内容和注释
* @NotNull，@NotEmpty会被展示为红色星号，表示必填参数

## Java 原生Interface文档预览

适用于各类使用`interface`作为接口的RPC服务，例如 Apache Dubbo。

返回的Java对象会被展示为类JSON的结构，继承，组合，泛型，递归等常见写法会被正确解析和拼合到结构中。

**由于RabiAPI是基于静态分析的，所以通过Jar包依赖的类暂时会以黄色感叹号显示**

<p align='center'><img src="/previews/java_interface.png"></p>

## Spring Boot 文档预览

支持使用`@RestController`的Spring接口，并且可以展示不同参数的类型

<p align='center'><img src="/previews/spring_boot.png"></p>

## Jax-RS 文档预览

Jax-RS是使用`@Path`注解标注的`interface`或`class`

<p align='center'><img src="/previews/jax_rs.png"></p>

## Markdown 导出效果预览

所有的接口类型(interface/spring/jax-rs)都可以导出为`markdown`格式

* 支持导出单个接口或实体类型到Markdown文档，复制到剪切板。
* 支持导出服务中所有的接口到Markdown文档，保存到文件。

<p align='center'><img src="/previews/markdown.png"></p>

## Asciidoc 导出效果预览

`asciidoc`也是一种轻量级标记语言，在表现效果上相对于`markdown`更加丰富，所有的接口类型(interface/spring/jax-rs)都可以导出为`asciidoc`格式

* 支持导出单个接口或实体类型到asciidoc文档
* 支持导出服务中所有的接口到asciidoc文档

<p align='center'><img src="/previews/asciidoc.png"></p>

## 接口搜索效果预览

RabiAPI支持通过

* 服务名称
* 服务的注释
* 接口名称
* 接口的注释
* 接口的请求路径（如果是HTTP接口）

来进行搜索，并高亮显示符合条件的结果

<p align='center'><img src="/previews/search_highlight.png"></p>

## 方法重载支持

方法重载是Java中常见的写法，即同名方法存在不同数量或类型的参数。

重载方法的上方会显示所有相关方法的Index。

<p align='center'><img src="/previews/overloads.png"></p>

## 实体类展示效果预览

RabiAPI支持把接口与接口使用的结构体分开展示，通过左侧选择栏过行切换。

<p align='center'><img src="/previews/structs.png"></p>

## 自动订阅条款和隐私政策

RabiAPI的功能需要订阅使用，每个订阅类型均有14天免费试用期，在试用期内可以随时取消订阅，不会收取任何费用.

同时在订阅前，您可以查看和使用示例文档，导出示例文档的内容，决定您是否适合使用该产品。

在您使用RabiAPI的过程中，我们不会收集您的任何数据。所有接口文档数据仅存在于您的本地环境。

您的订阅会按每月或每年自动续期，除非您提前 24 小时取消，订阅费将在您确认购买后从您的 iTunes 账户扣除。购买后，您可以在您的订阅设置中关闭。

使用条款

https://github.com/RabiAPI/RabiAPI-Support/blob/master/terms_of_service.md

隐私政策

https://github.com/RabiAPI/RabiAPI-Support/blob/master/privacy-policy.md
