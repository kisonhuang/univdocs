# Web服务器

## Web服务器

```java
## Web服务器
org.springframework.boot.web.server.WebServer
    + org.springframework.boot.web.embedded.tomcat.TomcatWebServer
    + org.springframework.boot.web.embedded.jetty.JettyWebServer
    + org.springframework.boot.web.embedded.netty.NettyWebServer
    + org.springframework.boot.web.embedded.undertow.UndertowWebServer
        + org.springframework.boot.web.embedded.undertow.UndertowServletWebServer

## 优雅关闭请求
## 优雅关闭请求回调
org.springframework.boot.web.server.GracefulShutdownCallback
## 优雅关闭请求结果
org.springframework.boot.web.server.GracefulShutdownResult

## Web服务器异常
org.springframework.boot.web.server.WebServerException
    + org.springframework.boot.web.server.PortInUseException
    + org.springframework.boot.web.embedded.tomcat.ConnectorStartFailedException

## Tomcat嵌入式Web应用类加载器
org.springframework.boot.web.embedded.tomcat.TomcatEmbeddedWebappClassLoader
## Jetty Servlet上下文初始化器配置
org.springframework.boot.web.embedded.jetty.ServletContextInitializerConfiguration
## Netty路由提供者
org.springframework.boot.web.embedded.netty.NettyRouteProvider
## Undertow HTTP处理器工厂
org.springframework.boot.web.embedded.undertow.HttpHandlerFactory
```

## Web服务器工厂

```java
## Web服务器工厂
org.springframework.boot.web.server.WebServerFactory
    + org.springframework.boot.web.server.ConfigurableWebServerFactory

## 错误页面注册表
org.springframework.boot.web.server.ErrorPageRegistry
    + org.springframework.boot.web.server.ConfigurableWebServerFactory
    + org.springframework.boot.web.servlet.support.ErrorPageFilter

## 可配置Web服务器工厂
+ org.springframework.boot.web.server.ConfigurableWebServerFactory
    + org.springframework.boot.web.embedded.tomcat.ConfigurableTomcatWebServerFactory
        + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
        + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
    + org.springframework.boot.web.embedded.jetty.ConfigurableJettyWebServerFactory
        + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
        + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
    + org.springframework.boot.web.embedded.undertow.ConfigurableUndertowWebServerFactory
        + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
        + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory
    + org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory
    + org.springframework.boot.web.reactive.server.ConfigurableReactiveWebServerFactory
    + org.springframework.boot.web.server.AbstractConfigurableWebServerFactory
        + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
        + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory

## Servlet服务器工厂
org.springframework.boot.web.servlet.server.ServletWebServerFactory
    + org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory

## Web监听器注册表
org.springframework.boot.web.servlet.WebListenerRegistry
    + org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory

## 可配置Servlet服务器工厂
+ org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory
    + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory

## 抽象的Servlet服务器工厂
+ org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
    + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
    + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
    + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory

## 响应式服务器工厂
org.springframework.boot.web.reactive.server.ReactiveWebServerFactory
    + org.springframework.boot.web.reactive.server.ConfigurableReactiveWebServerFactory

## 可配置响应式服务器工厂
+ org.springframework.boot.web.reactive.server.ConfigurableReactiveWebServerFactory
    + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory

## 抽象的响应式服务器工厂
+ org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory
    + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
    + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
    + org.springframework.boot.web.embedded.netty.NettyReactiveWebServerFactory
    + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory
```

## Web服务器工厂配置

```java
## 本地服务器端口
org.springframework.boot.web.server.LocalServerPort

## Web服务器工厂的配置
## 错误页面
org.springframework.boot.web.server.ErrorPage
## SSL配置
org.springframework.boot.web.server.Ssl
## 客户端认证策略
org.springframework.boot.web.server.Ssl.ClientAuth
## SSL密钥存储提供者
org.springframework.boot.web.server.SslStoreProvider
## HTTP/2配置
org.springframework.boot.web.server.Http2
## 压缩配置
org.springframework.boot.web.server.Compression
## Web服务器关闭策略
org.springframework.boot.web.server.Shutdown

## Servlet服务器工厂的配置
## 会话
org.springframework.boot.web.servlet.server.Session
## 会话跟踪模式
org.springframework.boot.web.servlet.server.Session.SessionTrackingMode
## Cookie
org.springframework.boot.web.server.Cookie
    + org.springframework.boot.web.servlet.server.Session.Cookie
## Cookie发送方式
org.springframework.boot.web.server.Cookie.SameSite
## mime类型映射
org.springframework.boot.web.server.MimeMappings
org.springframework.boot.web.server.MimeMappings.Mapping
## 临时
org.springframework.boot.web.servlet.ServletContextInitializer     临时
org.springframework.boot.web.servlet.server.Jsp                    临时
org.springframework.boot.web.servlet.server.CookieSameSiteSupplier 临时

## Tomcat服务器工厂的配置
## Tomcat上下文定制器
org.springframework.boot.web.embedded.tomcat.TomcatContextCustomizer
## Tomcat连接器定制器
org.springframework.boot.web.embedded.tomcat.TomcatConnectorCustomizer
## Tomcat协议处理器定制器
org.springframework.boot.web.embedded.tomcat.TomcatProtocolHandlerCustomizer

## Jetty服务器工厂的配置
## Jetty服务器定制器
org.springframework.boot.web.embedded.jetty.JettyServerCustomizer

## Netty服务器工厂的配置
## Netty服务器定制器
org.springframework.boot.web.embedded.netty.NettyServerCustomizer
    + org.springframework.boot.web.embedded.netty.SslServerCustomizer
## SSL配置验证器
org.springframework.boot.web.server.SslConfigurationValidator

## Undertow服务器工厂的配置
## Undertow构建器定制器
org.springframework.boot.web.embedded.undertow.UndertowBuilderCustomizer
## Undertow部署信息定制器
org.springframework.boot.web.embedded.undertow.UndertowDeploymentInfoCustomizer
```

## Web服务器工厂定制器

```java
## Web服务器工厂定制器
org.springframework.boot.web.server.WebServerFactoryCustomizer<T>
    + org.springframework.boot.autoconfigure.web.embedded.TomcatWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.embedded.JettyWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.embedded.NettyWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.embedded.UndertowWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.servlet.TomcatServletWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.servlet.UndertowServletWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.reactive.ReactiveWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.reactive.TomcatReactiveWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.websocket.servlet.TomcatWebSocketServletWebServerCustomizer
    + org.springframework.boot.autoconfigure.websocket.servlet.JettyWebSocketServletWebServerCustomizer
    + org.springframework.boot.autoconfigure.websocket.servlet.UndertowWebSocketServletWebServerCustomizer
    + org.springframework.boot.autoconfigure.websocket.reactive.TomcatWebSocketReactiveWebServerCustomizer
    + org.springframework.boot.actuate.autoconfigure.web.server.ManagementWebServerFactoryCustomizer<T>
```

## Web服务器工厂定制器属性

```java
## Web服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties

## Tomcat服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties.Tomcat
org.springframework.boot.autoconfigure.web.ServerProperties.Tomcat.Accesslog
org.springframework.boot.autoconfigure.web.ServerProperties.Tomcat.Threads
org.springframework.boot.autoconfigure.web.ServerProperties.Tomcat.Resource
org.springframework.boot.autoconfigure.web.ServerProperties.Tomcat.Mbeanregistry
org.springframework.boot.autoconfigure.web.ServerProperties.Tomcat.Remoteip

## Jetty服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties.Jetty
org.springframework.boot.autoconfigure.web.ServerProperties.Jetty.Accesslog
org.springframework.boot.autoconfigure.web.ServerProperties.Jetty.Accesslog.FORMAT
org.springframework.boot.autoconfigure.web.ServerProperties.Jetty.Threads

## Netty服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties.Netty

## Undertow服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties.Undertow
org.springframework.boot.autoconfigure.web.ServerProperties.Undertow.Accesslog
org.springframework.boot.autoconfigure.web.ServerProperties.Undertow.Threads
org.springframework.boot.autoconfigure.web.ServerProperties.Undertow.Options

## Servlet服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties.Servlet

## 响应式服务器属性
org.springframework.boot.autoconfigure.web.ServerProperties.Reactive
org.springframework.boot.autoconfigure.web.ServerProperties.Reactive.Session

## X-Forwarded-*头部的处理策略
org.springframework.boot.autoconfigure.web.ServerProperties.ForwardHeadersStrategy
```

## Web服务器工厂定制器的自动配置

```java
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration.TomcatWebServerFactoryCustomizerConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration.JettyWebServerFactoryCustomizerConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration.NettyWebServerFactoryCustomizerConfiguration
org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration.UndertowWebServerFactoryCustomizerConfiguration
```

## Web服务器工厂定制器的后置处理器

```java
org.springframework.boot.web.server.WebServerFactoryCustomizerBeanPostProcessor
```

## 错误页面注册器

```java
org.springframework.boot.web.server.ErrorPageRegistrar
```

## 错误页面注册器的后置处理器

```java
org.springframework.boot.web.server.ErrorPageRegistrarBeanPostProcessor
```




