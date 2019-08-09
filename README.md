# 概述

GodEye是一个基于micrometer的监控打点包，主要是对micrometer的metrcis打点进行增强扩展

# 功能
* 支持JVM metrcis打点
* 支持Http服务端请求进行metrcis打点
* 支持Tomcat metrcis打点
* 支持数据源（druid、hikaricp、shardingjdbc）连接池metrcis打点，并可以对SQL耗时进行打点
* 支持hazecast metrcis打点
* 支持rabbitmq、kafka metrcis打点
* 支持openfeign metrcis打点
* 支持redis连接池及redis command metrcis打点，包括（jedis、Lettuce）
* 支持resttemplate metrcis打点
* 支持Spring线程池打点
* 与kafka及skywalking集成，可以把日志全量的输到kafka中，在应用中可以不使用filebeat等收集工具来收集日志
* 规范化日志输出格式，让公司的日志标准统一
* 可自由与prometheus、influxdb集成

# 使用说明

  * 编译及构建
 
  ```
   mvn clean install
  ```

  * 将包deploy到公司的私有仓库中或直接引用中央仓库的包
