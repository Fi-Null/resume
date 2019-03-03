# 向科

**手机：** 185 0276 5806　　　　　　           **邮箱：** xk123401@gmail.com　　　　　**QQ/微信：** Fi-Null

**工作年限:**2年　　　　　　　　　　    	**期望薪资:**25-35k

------

## 教育经历

**华中科技大学**　　　　				**硕士**　　　　　 			**软件工程**　　　　　　　　      **2014-2017**

------

## 个人经历

**2016/03 - 至今**　　　　　　　　　  				**京东到家**　　　　　　　　  			**JAVA 开发工程师**

工作描述：主要负责订单中心、商家中心、合流墙系统、盘古系统、金额拆分系统、权限系统等核心项目的开发。

## 专业技能

- 扎实的Java编程基础，熟悉常用集合，JVM调优，多线程并发编程。
- 熟悉面向对象的相关设计模式，如模版方法模式、单例模式、责任链模式。
- 熟练使用Spring、SpringMVC、MyBatis等主流开源框架，并具备快速上手新型框架的能力。
- 熟悉高性能Netty网络编程，基于WebSocket协议实现长链接服务。
- 熟练使用MQ、Redis、Dubbo等分布式框架，有大型分布式系统开发经验。
- 熟悉MySql数据库，能够进行复杂的数据库表设计和Sql优化。
- 熟练使用ElasticSearch搭建搜索引擎，并提供复杂的多维度的信息检索能力。
- 熟练使用IDEA、Maven，Git等开发工具，熟悉Linux常用命令，具备简单Shell脚本编写能力。

------

## 项目经历										

- ### 订单中心系统

​	**项目介绍:**订单中心系统提供订单相关的各种操作，控制订单的生产流程。 订单中心系统包括Buffer，Core，Query。

​	Buffer主要用于接受提单系统的订单。使用Jsf Rpc框架提供远程调用服务，使用Tbschedule实时接收并控制订单的处理速率，对整个订单系统起着缓冲的作用。

​	Core提供订单相关的各种操作，控制订单的生产流程。其中订单补全使用线程池并行调用其他系统接口提高接口响应时间，使用Jsf Rpc框架提供远程服务给其他系统调用服务，使用Jmq完成系统的解藕和订单状态变更消息通知，使用Zookeeper做服务降级、动态配置和动态日志切换，使用Redis做分布式锁保证订单小号的连续性，使用Tbschedule实时处理失败数据保证订单数据的最终一致性。

​	Query提供订单信息各维度的检索能力。基于ElasticSearch开发的搜索服务，使用Jsf提供远程服务给其他系统调用，平均每天支撑上亿级的访问。

​	**我的职责:**在订单中心系统中，我主要负责以下几件事：

​	（1）优化订单小号的性能，具体提高了2-3倍

​	（2）使用模板方法模式重构订单补全逻辑，有利于程序的扩展

​	（3）使用线程池并行调用其他系统接口提高了接口的响应时间，Tp 999从2000ms下降到500ms

- ### 商家中心系统

​	**项目介绍:**商家中心系统提供商家操作订单的各种服务（接单，捡货，配送等核心操作）。商家中心系统包括商家中心Service，商家中心Web，长链接服务。

​	商家中心Service使用sf提供远程调用服务供开放平台商家使用，使用Jmq实现系统解藕和异步化。

​	商家中心Web基于Spring Mvc开发的Web应用，提供后台商家管理和操作页面，包括接单，打印，捡货，召唤配送，妥投，处理异常订单等操作，使用Jsf Rpc框架远程调用商家中心Service。

​	长链接服务基于Netty开发 ，使用Websocket协议与前端通讯，使用Zookeeper进行长链接服务器集群的管理，长链接服务主要用于自动打印和订单提醒。

​	**我的职责:**在商家中心系统中，我主要负责以下几件事：

​	（1）优化了商家中心Jvm，Young Gc Max由4000ms减低到50ms

​	（2）基于高性能网络框架Netty实现长链接服务，使用WebSocket协议与前端通讯，使用Zookeeper实现了长链接服务器集群化，实现系统的高可用。基于长链接服务，实现了Web自动打印和订单提醒。

- ### 合流墙系统

​	**项目介绍:**合流墙系统为全门店提供一套提升捡货效率的解决方案，支持按区拆分捡货任务，各区捡货任务合流到打包区捡货，大大提高了门店的捡货效率。合流墙系统拆分为合流墙service，合流墙web管理页面。

​	合流墙service负责提供合流墙的一些操作，包括接单、绑定袋子，捡货，合流、打包等服务。使用Jsf Rpc框架提供远程调用服务供其他系统调用，使用Jmq完成与其他系统的交互和解藕，使用Redis分布式锁保证数据的一致性。

​	合流墙web管理页面提供查看合流墙所有格子的状态、合流捡货单、合流单的详细信息等操作。系统基于Spring Mvc进行开发，使用Jsf Rpc框架远程调用合流墙service服务，并对返回数据进行加工、处理返回给前端展示。

​	**我的职责:**在合流墙系统中，我主要负责以下几件事：

​	（1）带领3人小团队，全权主导合流墙系统的架构设计和搭建。

​	（2）完成复杂数据库表的设计，实现核心流程的关键功能。
