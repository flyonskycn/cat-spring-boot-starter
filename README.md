# cat-spring-boot-starter

## 简介
> 在项目中快速引入Cat调用链监控。

## 项目依赖
cat-spring-boot-starter依赖于[autoconfigure项目](https://github.com/flyonskycn/autoconfigure)

## 使用步骤
### 引入依赖
```xml
<dependency>
    <groupId>org.flyonsky.boot</groupId>
    <artifactId>cat-spring-boot-starter</artifactId>
    <version>2.0.7.RELEASE</version>
</dependency>
```
### 在项目的resources/META-INF新建app.properties
app.properties内容如下：
app.name=timeclient
app.name设置与spring.application.name相同。

### 其它Cat相关配置参见Cat项目文档
[Cat项目](https://github.com/dianping/cat)

## 样例
[样例参考](https://github.com/flyonskycn/micro-service-study/tree/master/timeclient)
