# 介绍
---
***世界上没有两个相同的指纹***

fingerprint 产生于订单号的生成需求。在电商业务中订单号标志性一笔交易，所以订单号的生成规则从**性能**/**唯一性**/**高可用**等方面都有很高的要求。在我们的实际业务中，如果我们的唯一ID服务面向的是我们的微服务或者只是我们自己的应用
，那么便没有什么问题，我们可以通过使用UUID/redis/mysql等等的方法来实现，但是这些方法都会有些问题。
目前fingerprint作为分布式ID生成系统,高可用全局唯一ID生成器.已经被多家公司/机构/学校使用验证。

# 设计文档
---
//TODO

# SLA
---
在内网环境下，一般配置的容器单体可以达到**10W/s**