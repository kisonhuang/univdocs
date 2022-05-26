# Redis

## 启动器

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis</artifactId>
</dependency>

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis-reactive</artifactId>
</dependency>
```

## 自动配置

## Spring Data Redis的自动配置
org.springframework.boot.autoconfigure.data.redis.RedisAutoConfiguration
## Spring Data Redis Repository的自动配置
org.springframework.boot.autoconfigure.data.redis.RedisRepositoriesAutoConfiguration
## Spring Data响应式Redis的自动配置
org.springframework.boot.autoconfigure.data.redis.RedisReactiveAutoConfiguration


org.springframework.boot.autoconfigure.data.redis.ClientResourcesBuilderCustomizer
org.springframework.boot.autoconfigure.data.redis.JedisClientConfigurationBuilderCustomizer
org.springframework.boot.autoconfigure.data.redis.LettuceClientConfigurationBuilderCustomizer

## Redis配置属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties
## Redis客户端类型
org.springframework.boot.autoconfigure.data.redis.RedisProperties.ClientType
## Redis连接池属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Pool
## Redis集群属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Cluster
## Redis哨兵属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Sentinel
## Jedis客户端属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Jedis
## Lettuce客户端属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Lettuce
## Lettuce客户端集群属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Lettuce.Cluster
## Lettuce客户端集群刷新属性
org.springframework.boot.autoconfigure.data.redis.RedisProperties.Lettuce.Cluster.Refresh















































