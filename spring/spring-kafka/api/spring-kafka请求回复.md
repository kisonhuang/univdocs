# spring-kafka请求回复

## 操作

### 请求回复操作

```java
## 基本操作
The basic Kafka operations contract returning ListenableFutures
org.springframework.kafka.core.KafkaOperations<K, V>
    + org.springframework.kafka.core.KafkaTemplate<K, V>
        + org.springframework.kafka.requestreply.ReplyingKafkaTemplate<K, V, R>
            + org.springframework.kafka.requestreply.AggregatingReplyingKafkaTemplate<K, V, R>

## 请求回复操作
org.springframework.kafka.requestreply.ReplyingKafkaOperations<K, V, R>
    + org.springframework.kafka.requestreply.ReplyingKafkaTemplate<K, V, R>
        + org.springframework.kafka.requestreply.AggregatingReplyingKafkaTemplate<K, V, R>

## 请求回复操作
org.springframework.kafka.requestreply.ReplyingKafkaOperations<K, V, R>

## 请求回复操作模板
org.springframework.kafka.requestreply.ReplyingKafkaTemplate<K, V, R>

## 请求回复聚合操作模板：聚合具有相同关联ID的多个回复
org.springframework.kafka.requestreply.AggregatingReplyingKafkaTemplate<K, V, R>
```

## Future

### 请求回复Future

```java
## 请求回复可设置可监听Future
org.springframework.kafka.requestreply.RequestReplyFuture<K, V, R>
```

### 消息回复Future

```java
org.springframework.kafka.requestreply.RequestReplyMessageFuture<K, V>
    + org.springframework.kafka.requestreply.RequestReplyTypedMessageFuture<K, V, P>

## 消息回复的可设置可监听Future
org.springframework.kafka.requestreply.RequestReplyMessageFuture<K, V>

## 具有特定负载类型的消息回复的可设置可监听Future
org.springframework.kafka.requestreply.RequestReplyTypedMessageFuture<K, V, P>
```

## 关联

### 关联Key

```java
## 关联Key
org.springframework.kafka.requestreply.CorrelationKey
```

## 异常

### 回复超时异常

```java
## 回复超时异常
org.springframework.kafka.KafkaException
    + org.springframework.kafka.requestreply.KafkaReplyTimeoutException

## 在超时时间内未收到回复时的异常
org.springframework.kafka.requestreply.KafkaReplyTimeoutException
```




