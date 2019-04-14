DistributedLock
===============

redis分布式锁

* redis驱动信息 jedis 2.1.0
* redis版本信息 
* reids部署模式 集群还是单机，不知道集群和单机的api是否有区别，需要确认

实现引用 http://www.cnblogs.com/linjiqin/p/8003838.html

# 非常不幸
以上的方案有非常多的假设，具体的风险如下面引用的文章所述--主要是即使都满足也不行，GC的问题无法解决。目前来看，利用redis的场景只能用在低准确度要求的场景。
https://github.com/lilongthinker/JavaGuide/blob/master/docs/database/Redis/如何做可靠的分布式锁，Redlock真的可行么.md
