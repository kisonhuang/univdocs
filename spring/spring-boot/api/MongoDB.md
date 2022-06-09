# MongoDB

## 启动器

### 传统应用程序启动器

```xml
## 传统应用程序
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-mongodb</artifactId>
</dependency>
```

### 响应式应用程序启动器

```xml
## 响应式应用程序
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-mongodb-reactive</artifactId>
</dependency>
```

## 自动配置

### Mongo自动配置

```java
## Mongo自动配置
org.springframework.boot.autoconfigure.mongo.MongoAutoConfiguration
```

### 响应式Mongo自动配置

```java
## 响应式Mongo自动配置
org.springframework.boot.autoconfigure.mongo.MongoReactiveAutoConfiguration
```

### 嵌入式Mongo自动配置

```java
## 嵌入式Mongo自动配置
org.springframework.boot.autoconfigure.mongo.embedded.EmbeddedMongoAutoConfiguration
```

### Spring Data Mongo自动配置

```java
## Spring Data Mongo自动配置
org.springframework.boot.autoconfigure.data.mongo.MongoDataAutoConfiguration
```

### Spring Data 响应式Mongo自动配置

```java
## Spring Data响应式Mongo自动配置
org.springframework.boot.autoconfigure.data.mongo.MongoReactiveDataAutoConfiguration
```

### Spring Data Mongo Repository自动配置

```java
## Spring Data Mongo Repository自动配置
org.springframework.boot.autoconfigure.data.mongo.MongoRepositoriesAutoConfiguration
```

### Spring Data 响应式Mongo Repository自动配置

```java
## Spring Data 响应式Mongo Repository自动配置
org.springframework.boot.autoconfigure.data.mongo.MongoReactiveRepositoriesAutoConfiguration
```

## Bean工厂

### MongoClient工厂

```java
## MongoClient工厂
org.springframework.boot.autoconfigure.mongo.MongoClientFactorySupport<T>
    + org.springframework.boot.autoconfigure.mongo.MongoClientFactory
    + org.springframework.boot.autoconfigure.mongo.ReactiveMongoClientFactory

## MongoClient工厂基类
org.springframework.boot.autoconfigure.mongo.MongoClientFactorySupport<T>

## 阻塞式MongoClient工厂
org.springframework.boot.autoconfigure.mongo.MongoClientFactory

## 响应式MongoClient工厂
org.springframework.boot.autoconfigure.mongo.ReactiveMongoClientFactory
```

### MongoClient依赖对象的Bean工厂后置处理器

```java
## MongoClient依赖对象的Bean工厂后置处理器
org.springframework.boot.autoconfigure.AbstractDependsOnBeanFactoryPostProcessor
    + org.springframework.boot.autoconfigure.data.mongo.MongoClientDependsOnBeanFactoryPostProcessor
    + org.springframework.boot.autoconfigure.data.mongo.ReactiveStreamsMongoClientDependsOnBeanFactoryPostProcessor

## 使用嵌入式Mongo时，自动给MongoClient设置推荐依赖
org.springframework.boot.autoconfigure.data.mongo.MongoClientDependsOnBeanFactoryPostProcessor

## 使用嵌入式Mongo时，自动给MongoClient设置推荐依赖
org.springframework.boot.autoconfigure.data.mongo.ReactiveStreamsMongoClientDependsOnBeanFactoryPostProcessor
```

## 配置属性

### Mongo配置

```java
## Mongo配置
org.springframework.boot.autoconfigure.mongo.MongoProperties

## Mongo属性
spring.data.mongodb.uri
spring.data.mongodb.host
spring.data.mongodb.port
spring.data.mongodb.username
spring.data.mongodb.password
spring.data.mongodb.database
spring.data.mongodb.authentication-database
spring.data.mongodb.replica-set-name
spring.data.mongodb.auto-index-creation
spring.data.mongodb.uuid-representation
spring.data.mongodb.field-naming-strategy
spring.data.mongodb.repositories.type
```

### Mongo网格文件系统配置

```java
## Mongo网格文件系统配置
org.springframework.boot.autoconfigure.mongo.MongoProperties.Gridfs

## Mongo网格文件系统属性
spring.data.mongodb.gridfs.database
spring.data.mongodb.gridfs.bucket
```

### 嵌入式Mongo配置

```java
## 嵌入式Mongo配置
org.springframework.boot.autoconfigure.mongo.embedded.EmbeddedMongoProperties

## 嵌入式Mongo属性
spring.mongodb.embedded.version
```

### 嵌入式Mongo存储配置

```java
## 嵌入式Mongo存储配置
org.springframework.boot.autoconfigure.mongo.embedded.EmbeddedMongoProperties.Storage

## 嵌入式Mongo存储属性
spring.mongodb.embedded.storage.oplog-size
spring.mongodb.embedded.storage.database-dir
spring.mongodb.embedded.storage.repl-set-name
```

## 定制器

### MongoClientSettings.Builder定制器

```java
## MongoClientSettings.Builder定制器
org.springframework.boot.autoconfigure.mongo.MongoClientSettingsBuilderCustomizer
    + org.springframework.boot.autoconfigure.mongo.MongoPropertiesClientSettingsBuilderCustomizer

## Bean可以实现的回调接口
## 通过MongoClientSettings.Builder定制MongoClientSettings
## 同时保留默认的自动配置
org.springframework.boot.autoconfigure.mongo.MongoClientSettingsBuilderCustomizer

## 把MongoProperties应用于MongoClientSettings
org.springframework.boot.autoconfigure.mongo.MongoPropertiesClientSettingsBuilderCustomizer
```

### ImmutableDownloadConfig.Builder定制器

```java
## Bean可以实现的回调接口
## 通过ImmutableDownloadConfig.Builder定制DownloadConfig
## 同时保留默认的自动配置
org.springframework.boot.autoconfigure.mongo.embedded.DownloadConfigBuilderCustomizer
```

## 连接MongoDB

在Bean中注入以下Bean，可以连接MongoDB，默认连接的MongoDB服务器为mongodb://localhost/test：

```java
org.springframework.data.mongodb.MongoDatabaseFactory
```

连接MongoDB的依赖注入示例：

```java
@Component
public class SampleBean {

    private MongoDatabaseFactory mongoDatabaseFactory;

    public SampleBean(MongoDatabaseFactory mongoDatabaseFactory) {
        this.mongoDatabaseFactory = mongoDatabaseFactory;
    }

}
```




