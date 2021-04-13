# opensource-log-manager-solution
log solution，elk (Elasticsearch Logstash Kibana)，efk (Elasticsearch Filebeats Kibana)

# ELk

ELK 是 Elastic 公司提供的一套完整的日志收集以及展示的解决方案，是三个产品的首字母缩写，分别是 Elasticsearch、Logstash 和 Kibana。

![image](https://user-images.githubusercontent.com/13504729/114493119-82276700-9c4c-11eb-8c5f-80b861e555ab.png)


* Logstash 的主要作用是收集分布在各处的 log 并进行处理；
* Elasticsearch 则是一个集中存储 log 的地方，更重要的是它是一个全文检索以及分析的引擎，它能让用户以近乎实时的方式来查看、分析海量的数据。
* Kibana 则是为 Elasticsearch 开发的前端 GUI，让用户可以很方便的以图形化的接口查询 Elasticsearch 中存储的数据，同时也提供了各种分析的模块，比如构建 dashboard 的功能。

![image](https://user-images.githubusercontent.com/13504729/114493028-560be600-9c4c-11eb-89e8-6daa3d15e798.png)

Logstash 则并不是唯一的收集 log 的方案，Fluentd 和 Filebeats 也能用于收集 log。所以现在网上有 ELK，EFK 之类的缩写。

由于Logstash 在数据收集上并不出色，而且作为 Agent，其性能并不达标。基于此，Elastic 发布了 beats 系列轻量级采集组件。

![image](https://user-images.githubusercontent.com/13504729/114493209-b733b980-9c4c-11eb-9e0b-a94ff0636b13.png)
