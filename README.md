# 介绍

INTRODUCE
---
***世界上没有两个相同的指纹***

***There are no two identical fingerprints in the world***

fingerprint 产生于订单号的生成需求。在电商业务中订单号标志性一笔交易，所以订单号的生成规则从**性能**/**唯一性**/**高可用**等方面都有很高的要求。在我们的实际业务中，如果我们的唯一ID服务面向的是我们的微服务或者只是我们自己的应用
，那么便没有什么问题，我们可以通过使用UUID/redis/mysql等等的方法来实现，但是这些方法都会有些问题。
目前fingerprint作为分布式ID生成系统,高可用全局唯一ID生成器.已经被多家公司/机构/学校使用验证。

The fingerprint is generated from the generation request of the order number. In the e-commerce business, the order number is a landmark transaction, so the generation rules of the order number have high requirements in terms of performance, uniqueness, and high availability. In our actual business, if our unique ID service is oriented to our microservices or just our own applications, then there is no problem. We can achieve this by using UUID/redis/mysql, etc., but These methods will have some problems. Fingerprint is currently used as a distributed ID generation system, a highly available globally unique ID generator. It has been verified by many companies/institutions/schools.

# 设计文档

Design document
---
## 设计目标（Design goals）

* 接入简单：提供http接入能力以及方便公司rpc集成 （Simple access: provide http access capability and facilitate company rpc integration）
* 高可用：即时部分fingerprint服务宕机或者存储注入mysql宕机也能提供一段时间服务 （High availability: Even if part of the fingerprint service is down or storage injection mysql is down, it can provide services for a period of time）
* 高并发：支持10W+QPS起 （High concurrency: support from 10W+QPS）
* 趋势递增：支持生成ID的趋势递增 （Increasing trend: Support the increasing trend of ID generation）
* 低延时：在高并发特性的基础上rt控制在1ms以内 （Low latency: rt is controlled within 1ms on the basis of high concurrency）
 
## 

# SLA
---
在内网环境下，一般配置的容器单体可以达到**10W/s**

In the internal network environment, the general configuration of the container monomer can reach 10W/s
