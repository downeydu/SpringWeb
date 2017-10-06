## 第一章 Spring 概述 (上)
代码:spring1
### 1 Spring 是什么?
>The Spring Framework  is a lightweght solution and a  potential  one-stop-shop for building your enterprise-ready application.

>Spring 是 轻量级,一站式,开发框架.
* 轻量级:相对于老的JAVA EE 的 EJB框架
* 一站式:将各种工具中整合到一起


###  2 Spring历史
* 2002 Rod Johnson 创建
* 2004 1.0 核心功能
* 2006 2.0 支持AOP
* 2007 2.5 支持annotation
* 2009 3.0 
* 2013 4.0 支持java 8 
<br>.......
* 2017 Spring 5.0 
* 2017 Spring Boot -> Spring cloud -> Spring Data Flow

### 3 为什么要用Spring框架?
* Inversion of Control (Ioc 控制反转)
* Aspect-Oriented Programing (AOP 面向切面变成)


#### 3.1 Ioc 控制反转

* 谁来控制 - 螺丝刀生产商
* 控制什么 - 螺丝刀到头

现实场景:我们需要螺丝刀,但是随场景变化螺丝刀有一字或者十字,螺丝刀的大小可能也会改变,所以我们就发明了螺丝刀的套装,可以变更螺丝刀头.
<hr>

程序层面的解释:
* 谁来控制 - IOC容器
* 控制什么 - 对象的依赖(Dependency inception ,依赖注入[^1] )


#### 3.2 AOP 面向切面变成

日志的场景,通常会把日志程序加载在业务逻辑中.造成代码不友好,可维护性低.
* AOP 的目的:业务逻辑和非业务逻辑分离.运行时整合.
* 常用场景:日志,安全.


### Spring 框架模块图
1. **核心容器** 
    1. 对象创建,专配
    2. 对象生命周期管理
    3. 对象上下文环境管理
2. **AOP**
    1. AOP支持
    2. AspectJ支持
3. **数据访问**
    1. JDBC
    2. 事务支持
    3. ORM整合(对象关系映射)
4. **Web**
    1. MVC框架
    2. web工具支持(上传下载...)
    3. 模版支持(freemarker,jsp)
5. **Test**
    1. 测试模块

























[^1]: 很多时候,会将IOC 和 DI 等同,实际上 DI是目的,IOC是实现方式.