---
title: Spring Cloud 001
tags: Spring Cloud
renderNumberedHeading: true
grammar_cjkRuby: true
---

1、Spring Cloud 并不是一个具体的框架，大家可以把它理解为一个工具箱，它提供的各类 工具，可以帮助我们快速的构建分布式系统。 

2、Spring Cloud 还包括以下几个重要的模块： 
a、Spring Cloud Config：为分布式系统提供了配置服务器和配置客户端，通过对它们的配置，可以很好的管理集群中的配置文件。 
b、Spring Cloud Sleuth：服务跟踪框架，可以与 Zipkin、Apache HTrace 和 ELK 等数据分析、服务跟踪系统进行整合，为服务跟踪、解决问题提供了便利。 
c、Spring Cloud Stream：用于构建消息驱动微服务的框架，该框架在 Spring Boot 的基础上，整合了“Spring Integration”来连接消息代理中间件。 
d、Spring Cloud Bus：连接 RabbitMQ、Kafka 等消息代理的集群消息总线。
e、Spring Cloud Netflix

3、Spring Cloud 的各个项目基于 Spring Boot，将 Netflix 的多个框架进行封装，并且通过自动配置的方式将这些框架绑定到 Spring 的环境中，从而简化了这些框架的使用。由于Spring Boot 的简便，使得我们在使用 Spring Cloud 时，很容易的将 Netflix 各个框架整合进我们的项目中。Spring Cloud 下的“Spring Cloud Netflix”模块，主要封装了 Netflix 的以 
下项目：
1)、Eureka：基于 REST 服务的分布式中间件，主要用于服务管理。 
2)、Hystrix：容错框架，通过添加延迟阀值以及容错的逻辑，来帮助我们控制分布式系统间组件的交互。 
3)、Feign：一个 REST 客户端，目的是为了简化 Web Service 客户端的开发 
4)、Ribbon：负载均衡框架，在微服务集群中为各个客户端的通信提供支持，它主要实现中间层应用程序的负载均衡 
5)、Zuul：为微服务集群提供过代理、过滤、路由等功能。
