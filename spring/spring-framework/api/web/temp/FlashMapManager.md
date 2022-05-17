# FlashMapManager

```java
org.springframework.web.servlet.FlashMapManager
    + org.springframework.web.servlet.support.AbstractFlashMapManager
        + org.springframework.web.servlet.support.SessionFlashMapManager

org.springframework.web.servlet.FlashMap
```

## FlashMapManager

查找并保存FlashMap实例

```java

```

## AbstractFlashMapManager

```java

```

## SessionFlashMapManager

```java

```

## FlashMap

```java
## 请求路径
String targetRequestPath          标识FlashMap请求的请求路径
setTargetRequestPath(String path) 设置请求路径
String getTargetRequestPath()     获取请求路径

## 请求参数
MultiValueMap<String, String> targetRequestParams            标识FlashMap请求的请求参数
addTargetRequestParams(MultiValueMap<String, String> params) 添加请求参数
addTargetRequestParam(String name, String value)             添加请求参数
getTargetRequestParams()                                     获取请求参数

## 过期时间
long expirationTime = -1               过期时间（毫秒），默认为-1（永不过期）
startExpirationPeriod(int timeToLive)  设置过期期限（秒）
setExpirationTime(long expirationTime) 设置过期时间（毫秒）
getExpirationTime()                    获取过期时间（毫秒）
isExpired()                            判断是否过期
```




