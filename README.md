<img src="doc/assets/img/logo-small.png">

#### **[Quickstart](#quickstart)** • **[Examples](#the-demo)** • **[Landscape](#landscape-of-central-platform)** • **[Chat with us](https://gitter.im/cp-ddd-framework/community)**

[![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](https://github.com/funkygao/cp-ddd-framework/blob/master/LICENSE)
[![CI](https://github.com/funkygao/cp-ddd-framework/workflows/CI/badge.svg?branch=master)](https://github.com/funkygao/cp-ddd-framework/actions?query=branch%3Amaster+workflow%3ACI)
[![Code Quality: Java](https://img.shields.io/lgtm/grade/java/g/funkygao/cp-ddd-framework.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/funkygao/cp-ddd-framework/context:java)
[![Coverage Status](https://img.shields.io/codecov/c/github/funkygao/cp-ddd-framework.svg)](https://codecov.io/gh/funkygao/cp-ddd-framework)
[![TODO](https://badgen.net/https/api.tickgit.com/badgen/github.com/funkygao/cp-ddd-framework?label=todos)](https://www.tickgit.com/browse?repo=github.com/funkygao/cp-ddd-framework)
[![Ask Us Anything !](https://img.shields.io/badge/Ask%20us-anything-1abc9c.svg)](https://gitter.im/cp-ddd-framework/community)

# cp-ddd-framework

<details>
<summary><b>Table of content</b></summary>

## Table of content
   * [What is cp-ddd-framework](#what-is-cp-ddd-framework)
      * [Current status](#current-status)
      * [Requirements](#requirements)
      * [Quickstart](#quickstart)
      * [What problems does it solve](#what-problems-does-it-solve)
      * [Modules](#modules)
      * [Key abstractions](#key-abstractions)
   * [Using cp-ddd-framework](#using-cp-ddd-framework)
      * [Maven](#maven)
      * [Gradle](#gradle)
      * [Building from Source](#building-from-source)
   * [The Demo](#the-demo)
   * [Reference documentation](#reference-documentation)
   * [FAQ](#faq)
   * [Landscape of Central Platform](#landscape-of-central-platform)
   * [Contribution](#contribution)
   * [Licensing](#licensing)

</details>

----

## What is cp-ddd-framework?

cp-ddd-framework, also known as DDDplus, is a lightweight flexible development framework for complex business architecture.

一套轻量级业务中台开发框架，以[DDD](https://github.com/funkygao/cp-ddd-framework/wiki/DDD)思想为基础，致力于业务资产的可沉淀和可传承，全方位解决复杂业务场景的扩展问题，实现[中台核心要素](https://github.com/funkygao/cp-ddd-framework/wiki/%E4%B8%9A%E5%8A%A1%E4%B8%AD%E5%8F%B0%E7%9A%84%E6%A0%B8%E5%BF%83%E8%A6%81%E7%B4%A0)，赋能中台建设。

融合了前中台复杂生态协作方法论，充分考虑组织架构、技术债、学习门槛、可演进性、运维和落地成本以及风险而开发的，面向复杂业务场景架构设计，重新定义业务开发，是中台架构的顶层设计和完整解决方案。

Note: cp means Central Platform：中台。
### Current status

Used for several complex critical central platform projects in production environment.

多个复杂的中台核心项目生产环境下使用。

### Requirements

Requires Java 1.8+ and Spring 4.3.12.RELEASE or later.

### Quickstart

[快速入门](https://github.com/funkygao/cp-ddd-framework/wiki)。

Please visit [Quickstart](https://github.com/funkygao/cp-ddd-framework/wiki).

### What problems does it solve

- born for extension, the OCP
- 业务逻辑的扩展：uncertain biz logic
- 业务流程的扩展：uncertain biz flow
- 业务模型的扩展：uncertain biz model
- 业务的多态：polymorphic business
- 业务前台与中台如何协同：synergy between BP and CP teams
- 如何让中台架构特色的DDD稳稳当当落地：DDD seamlessly landing in code
- 如何降低系统实现的复杂度：reduce entropy of the system
- empower the system to evolve without corruption
- 普通研发如何编写出优雅的业务代码：low threshold for average developer to build elegant biz code
- and more

### Modules

```
cp-ddd-framework
   ├── dddplus-spec    - Specification of the framework
   ├── dddplus-runtime - Runtime implementation
   ├── dddplus-plugin  - Plugin hot reloading mechanism
   ├── dddplus-unit    - Extra unit test facilities
   ├── dddplus-enforce - Enforce expected evolvement of the business architecture
   └── dddplus-test    - Fully covered unit test cases
```

### Key abstractions

14个核心抽象勾勒出业务中台的骨架，以不变应万变。

![](http://www.plantuml.com/plantuml/svg/XLHDRnCn4BtxLunwQW-fn3LQLIq4f1v0LSiTJUn9rehNZkpPfAZqlpDE7DWF8tAAvxrvyxttYJ5otpcLTjRlCM87BNfpZ9QPF6pG9HfWgKKJZjPlc-PekVrnVj_T0SUUbACD0mU8Tjio61j9imrUgJtg7Mu9dbo_jHwQvek8aRYzAP2VzKnnWvhWyT6GPyi_doa5Tw0unLUXG-i_lpBv9D9JE0V0jQEf_Mimv1wOKRSTUHR_cJ1fQ-Y5QPykg7QO4ZmX2ycFB94zHVMkb0zCSDK6XaWkeCcnhm0JVFkWIh6tj_cXPZMyK3nOJHL0Sb23_x04UYNTCrtV3DdFT0Yx773eLZ6AVmpEhMK68l2dHT3yMYnc3PtXiu5KUddASEz4HmBKyKZUK1GOruaZQeRIQjBVgHDVfh_GHqmb_uUrTH9SpImYkIM-f2rngvIDZUc_94CRxDs8DijjD8FLQYNljyJ8LhzB46-AMXqygGaqsR4SkXWAFksrC3fatLwNAPqwUwFKU8FAeEhBKy3ghinLAfrNqmqfYkDQwgpgtStBF7FBdVqJBaTN6M4ZiBHzN7QnLHAhbRa45pGoLVYBnTqbjoMiPPnrIiclKDIdu5au525BeybNbSzZY6ItixsGb2egyjR1a2fnotCUkDWh-vgr1_rOGeYwfSHHG7LFtkHl_cy0)

## Using cp-ddd-framework

Latest version [0.1.1](https://github.com/funkygao/cp-ddd-framework/releases/tag/v0.1.1)，已推送至Maven中央库，可直接引入。

### Maven

```xml
<properties>
    <dddplus.version>0.1.1</dddplus.version>
</properties>

<dependency>
    <groupId>io.github.dddplus</groupId>
    <artifactId>dddplus-runtime</artifactId>
    <version>${dddplus.version}</version>
</dependency>
```

### Gradle

```groovy
dependencies {
    ...
    compile 'io.github.dddplus:dddplus-runtime:0.1.1'
}
```

### Building from Source

``` bash
git clone https://github.com/funkygao/cp-ddd-framework.git
cd cp-ddd-framework/
mvn install # will run all test cases
```

## The Demo

Please visit [使用该框架搭建`订单履约中台`的例子](https://github.com/dddplus/dddplus-demo).

## Reference documentation

Please visit [Javadoc](https://funkygao.github.io/cp-ddd-framework/doc/apidocs/).

## FAQ

Please visit [FAQ](https://github.com/funkygao/cp-ddd-framework/wiki/FAQ).

## Landscape of Central Platform

业务中台建设全景图。

![](doc/assets/img/landscape.png)

## Contribution

You are welcome to contribute to the project with pull requests on GitHub.

If you find a bug or want to request a feature, please use the [Issue Tracker](https://github.com/funkygao/cp-ddd-framework/issues).

For any question, you can use [Gitter Chat](https://gitter.im/cp-ddd-framework/community) to ask.

## Licensing

cp-ddd-framework is licensed under the Apache License, Version 2.0 (the "License"); you may not use this project except in compliance with the License. You may obtain a copy of the License at [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0).
