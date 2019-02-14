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
### 配置Cat的服务器地址配置
1. 新建/data/appdatas/cat目录,确保启动程序的用户对其具有读写权限。
2. 新建/data/applogs/cat目录,  确保启动程序的用户对其具有读写权限。Cat日志会输出到本目录。
3. 新建/data/appdatas/cat/client.xml文件。
```xml
<?xml version="1.0" encoding="utf-8"?>
<config xmlns:xsi="http://www.w3.org/2001/XMLSchema" xsi:noNamespaceSchemaLocation="config.xsd">
    <servers>
        <server ip="<cat server ip address>" port="2280" http-port="8080" />
    </servers>
</config>
```
> 记录修改IP地址为Cat服务器的地址
[详细信息参见](https://github.com/dianping/cat/blob/master/lib/_/preparations.md)
### 在项目的resources/META-INF新建app.properties
app.properties内容如下：
app.name=timeclient
最佳实践:app.name设置与spring.application.name相同。

### 其它Cat相关配置参见Cat项目文档
[Cat项目](https://github.com/dianping/cat)

## 样例
[样例参考](https://github.com/flyonskycn/micro-service-study/tree/master/timeclient)
