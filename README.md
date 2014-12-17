jdbc-cas4-overlay-template
============================

Generic CAS maven war overlay + JDBC

使用mysql数据库提供用户数据的cas服务器模板

# 版本
```xml
<cas.version>4.0.0</cas.version>
```

# 环境需求
* JDK 1.7+
* Apache Maven 3+
* Servlet container supporting Servlet 3+ spec (e.g. Apache Tomcat 7+)

# 配置
把下面的配置复制到`/etc/cas`文件夹里面，在`/var/log/`里面创建`cas`文件夹并赋予运行Servlet容器的用户读写的权限

* `cas.properties`
* `log4j.xml`

# 发布

* 运行 `mvn clean package`
* 把 `target/cas.war` 复制到Servlet容器的webapp目录
