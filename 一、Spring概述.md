[TOC]

## 一、Spring概述

### 1.1 Spring是什么

Spring是一个分层的Java SE/EE**全栈式轻量级**开源框架，
**full-stack（全栈式）**：对各种主流技术和框架都进行了整合，同时对三层架构都提供解决方案。
**轻量级**：轻量级和重量级的划分主要依据就是看它使用了多少服务，启动时需要加载的资源以及耦合度等等。

***Spring涵盖：***
**表现层**：SpringMVC
**持久层**：Spring JDBC Template
**业务层**：事务管理等企业级技术
<u>Spring能整合众多第三方框架（如Hibernate、MyBatis），已成为Java EE企业应用中最广泛使用的开源框架。</u>
**两大核心机制：**
***IOC***（Inverse of Control，控制反转）：把对象的创建权交给Spring
***AOP***（Aspect Oriented Programming，面向切面编程）：在不修改源码的情况下对方法进行增强。



### 1.2 Spring发展历程

****

> *** EJB**
>
> 1997 年，IBM提出了EJB 的思想
>
> 1998 年，SUN制定开发标准规范 EJB1.0
>
> 1999 年，EJB1.1 发布
>
> 2001 年，EJB2.0 发布
>
> 2003 年，EJB2.1 发布
>
> 2006 年，EJB3.0 发布
>
> *** Spring**
>
> **Rod Johnson（Spring 之父）**-- 改变Java世界的大师级人物
>
> 2002年编著《Expert one on one J2EE design and development》
>
> 指出Java EE和EJB组件框架中的主要缺陷，提出基于普通Java类依赖注入的简化解决方案。
>
> 2004年编著《Expert one-on-one J2EE Development without EJB》
>
> 阐述不使用EJB的Java EE开发方式（Spring雏形），同年4月，Spring 1.0正式发布
>
> 2006年10月，发布 Spring 2.0
>
> 2009年12月，发布 Spring 3.0
>
> 2013年12月，发布 Spring 4.0
>
> 2017年9月，发布 Spring 5.0 通用版（GA）

### 1.3 Spring优势

**（1）方便解耦，简化开发**

Spring作为容器，统一管理对象的创建和依赖关系。

**耦合度**指对象间的关联程度，高耦合会导致修改一个对象需同步修改其他对象，增加维护成本。Spring通过IoC降低耦合。

![spring优点](https://github.com/gvc10233/note_images/blob/main/spring_img/spring0101.png)

**（2）AOP编程支持**

提供面向切面编程能力，方便实现程序进行权限拦截，运行监控等功能。

**（3）声明式事务支持**

通过配置完成事务的管理，无需手动编程。

**（4）方便测试，降低JavaEE API的使用**

集成JUnit4支持注解测试，封装JavaEE API，降低使用复杂度。

**（5）优秀框架集成**

兼容主流开源框架（如MyBatis、Hibernate），并提供直接支持。

**1.4 Spring体系结构**

