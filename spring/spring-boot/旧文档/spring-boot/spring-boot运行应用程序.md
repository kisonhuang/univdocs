# Spring Boot依赖

## 运行应用程序

### 运行打包后的应用程序

```shell
$ java -jar target/myapplication-0.0.1-SNAPSHOT.jar
```

```shell
$ java -Xdebug -Xrunjdwp:server=y,transport=dt_socket,address=8000,suspend=n -jar target/myapplication-0.0.1-SNAPSHOT.jar
```

### 使用Maven插件

```shell
$ mvn spring-boot:run
```

```shell
$ export MAVEN_OPTS=-Xmx1024m
```

















