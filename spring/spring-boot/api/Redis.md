# Redis

## 启动器

### 传统应用程序启动器

```xml
## 传统应用程序，默认使用Lettuce
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis</artifactId>
</dependency>
```

### 响应式应用程序启动器

```xml
## 响应式应用程序
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis-reactive</artifactId>
</dependency>
```

## 自动配置

### Spring Data Redis自动配置

```java
## Spring Data Redis自动配置：
## 配置Bean：RedisTemplate
## 配置Bean：StringRedisTemplate
## 配置Bean：JedisConnectionFactory  （使用Jedis客户端）
## 配置Bean：DefaultClientResources  （使用Lettuce客户端）
## 配置Bean：LettuceConnectionFactory（使用Lettuce客户端）
org.springframework.boot.autoconfigure.data.redis.RedisAutoConfiguration
```

### Spring Data Redis Repository自动配置

```java
## Spring Data Redis Repository自动配置
org.springframework.boot.autoconfigure.data.redis.RedisRepositoriesAutoConfiguration
```

### Spring Data 响应式Redis自动配置

```java
## Spring Data响应式Redis自动配置
org.springframework.boot.autoconfigure.data.redis.RedisReactiveAutoConfiguration
```

## 配置属性

### Redis配置

```java
## Redis配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties
## Redis连接池配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Pool
## Redis客户端类型
org.springframework.boot.autoconfigure.data.redis.RedisProperties.ClientType

## Redis属性
spring.redis.url
spring.redis.host
spring.redis.port
spring.redis.username
spring.redis.password
spring.redis.database
spring.redis.ssl
spring.redis.timeout
spring.redis.connect-timeout
spring.redis.client-name
spring.redis.client-type
```

### Redis集群配置

```java
## Redis集群配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Cluster

## Redis集群属性
spring.redis.cluster.nodes
spring.redis.cluster.max-redirects
```

### Redis哨兵配置

```java
## Redis哨兵配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Sentinel

## Redis哨兵属性
spring.redis.sentinel.master
spring.redis.sentinel.nodes
spring.redis.sentinel.username
spring.redis.sentinel.password
```

### Jedis客户端配置

```java
## Jedis客户端配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Jedis

## Jedis客户端属性
spring.redis.jedis.pool.enabled
spring.redis.jedis.pool.min-idle
spring.redis.jedis.pool.max-idle
spring.redis.jedis.pool.max-active
spring.redis.jedis.pool.max-wait
spring.redis.jedis.pool.time-between-eviction-runs
```

### Lettuce客户端配置

```java
## Lettuce客户端配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Lettuce
## Lettuce客户端集群配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Lettuce.Cluster
## Lettuce客户端集群刷新配置
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Lettuce.Cluster.Refresh

## Lettuce客户端属性
spring.redis.lettuce.pool.enabled
spring.redis.lettuce.pool.min-idle
spring.redis.lettuce.pool.max-idle
spring.redis.lettuce.pool.max-active
spring.redis.lettuce.pool.max-wait
spring.redis.lettuce.pool.time-between-eviction-runs
spring.redis.lettuce.shutdown-timeout

## Lettuce客户端集群刷新属性
spring.redis.lettuce.cluster.refresh.dynamic-refresh-sources
spring.redis.lettuce.cluster.refresh.period
spring.redis.lettuce.cluster.refresh.adaptive
```

## 定制器

### ClientResources.Builder定制器

```java
## Bean可以实现的回调接口
## 通过ClientResources.Builder定制ClientResources
## 同时保留默认的自动配置
org.springframework.boot.autoconfigure.data.redis.ClientResourcesBuilderCustomizer
```

### JedisClientConfigurationBuilder定制器

```java
## Bean可以实现的回调接口
## 通过JedisClientConfiguration.JedisClientConfigurationBuilder定制JedisClientConfiguration
## 同时保留默认的自动配置
org.springframework.boot.autoconfigure.data.redis.JedisClientConfigurationBuilderCustomizer
```

### LettuceClientConfigurationBuilder定制器

```java
## Bean可以实现的回调接口
## 通过LettuceClientConfiguration.LettuceClientConfigurationBuilder定制LettuceClientConfiguration
## 同时保留默认的自动配置
org.springframework.boot.autoconfigure.data.redis.LettuceClientConfigurationBuilderCustomizer
```

## 连接Redis

在Bean中注入以下Bean，可以连接Redis，默认连接的Redis服务器为localhost:6379：

```java
org.springframework.data.redis.core.RedisTemplate
org.springframework.data.redis.core.StringRedisTemplate
org.springframework.data.redis.connection.RedisConnectionFactory
```

连接Redis的依赖注入示例：

```java
@Component
public class SampleBean {

    private StringRedisTemplate stringRedisTemplate;

    public SampleBean(StringRedisTemplate stringRedisTemplate) {
        this.stringRedisTemplate = stringRedisTemplate;
    }

}
```

注册以下Bean可以完全控制Redis的配置：

```java
org.springframework.data.redis.connection.RedisStandaloneConfiguration
org.springframework.data.redis.connection.RedisClusterConfiguration
org.springframework.data.redis.connection.RedisSentinelConfiguration
```

添加任何自动配置类型的@Bean，都会替换默认Bean。
除非是基于Bean名称redisTemplate，而不是Bean类型排除RedisTemplate的情况。

类路径中存在commons-pool2时，会自动配置连接池工厂。




