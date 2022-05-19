# SpringApplication

## SpringBootApplication

```java
org.springframework.boot.autoconfigure.SpringBootApplication

org.springframework.boot.SpringBootConfiguration

org.springframework.boot.autoconfigure.EnableAutoConfiguration
org.springframework.boot.autoconfigure.AutoConfigurationPackage
org.springframework.boot.autoconfigure.AutoConfigurationPackages
org.springframework.boot.autoconfigure.AutoConfigurationImportSelector

org.springframework.boot.context.TypeExcludeFilter
    + org.springframework.boot.test.autoconfigure.filter.AnnotationCustomizableTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.filter.StandardAnnotationCustomizableTypeExcludeFilter<A>
            + org.springframework.boot.test.autoconfigure.data.jdbc.DataJdbcTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.orm.jpa.DataJpaTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.data.ldap.DataLdapTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.data.mongo.DataMongoTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.data.neo4j.DataNeo4jTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.data.redis.DataRedisTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.jdbc.JdbcTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.jooq.JooqTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.json.JsonTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.web.client.RestClientTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.web.reactive.WebFluxTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.web.servlet.WebMvcTypeExcludeFilter
            + org.springframework.boot.test.autoconfigure.webservices.client.WebServiceClientExcludeFilter
            + org.springframework.boot.test.autoconfigure.webservices.server.WebServiceServerTypeExcludeFilter

org.springframework.boot.autoconfigure.AutoConfigurationExcludeFilter
```

## SpringApplication

```java
org.springframework.boot.SpringApplication

org.springframework.boot.SpringApplicationRunListener
    + org.springframework.boot.context.event.EventPublishingRunListener

org.springframework.boot.SpringApplicationShutdownHandlers

org.springframework.boot.SpringBootExceptionReporter
org.springframework.boot.SpringBootVersion

org.springframework.boot.Banner
   + org.springframework.boot.ImageBanner
   + org.springframework.boot.ResourceBanner

org.springframework.boot.Banner.Mode
org.springframework.boot.ImageBanner.PixelMode

org.springframework.boot.BootstrapRegistryInitializer

org.springframework.boot.BootstrapContext
    + org.springframework.boot.ConfigurableBootstrapContext
        + org.springframework.boot.DefaultBootstrapContext

org.springframework.boot.BootstrapRegistry
    + org.springframework.boot.ConfigurableBootstrapContext
        + org.springframework.boot.DefaultBootstrapContext

org.springframework.boot.BootstrapRegistry.Scope
org.springframework.boot.BootstrapRegistry.InstanceSupplier

org.springframework.boot.BootstrapContextClosedEvent

org.springframework.boot.WebApplicationType
org.springframework.boot.ApplicationContextFactory

org.springframework.boot.ApplicationRunner
    + org.springframework.boot.autoconfigure.batch.JobLauncherApplicationRunner

org.springframework.boot.ApplicationArguments
    + org.springframework.boot.DefaultApplicationArguments

org.springframework.boot.CommandLineRunner

org.springframework.boot.DefaultPropertiesPropertySource

org.springframework.boot.ExitCodeEvent
org.springframework.boot.ExitCodeExceptionMapper

org.springframework.boot.ExitCodeGenerator
    + org.springframework.boot.autoconfigure.batch.JobExecutionExitCodeGenerator

org.springframework.boot.LazyInitializationBeanFactoryPostProcessor
org.springframework.boot.LazyInitializationExcludeFilter
```

## SpringApplicationEvent

```java
org.springframework.boot.context.event.SpringApplicationEvent
    + org.springframework.boot.context.event.ApplicationStartingEvent
    + org.springframework.boot.context.event.ApplicationEnvironmentPreparedEvent
    + org.springframework.boot.context.event.ApplicationContextInitializedEvent
    + org.springframework.boot.context.event.ApplicationPreparedEvent
    + org.springframework.boot.context.event.ApplicationStartedEvent
    + org.springframework.boot.context.event.ApplicationFailedEvent
    + org.springframework.boot.context.event.ApplicationReadyEvent
```

## server

```java
org.springframework.boot.web.server.WebServerFactory
    + org.springframework.boot.web.server.ConfigurableWebServerFactory
        + org.springframework.boot.web.server.AbstractConfigurableWebServerFactory
            + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
            + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.netty.NettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory
        + org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory
            + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
        + org.springframework.boot.web.reactive.server.ConfigurableReactiveWebServerFactory
            + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.netty.NettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory
        + org.springframework.boot.web.embedded.jetty.ConfigurableJettyWebServerFactory
            + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
            + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
        + org.springframework.boot.web.embedded.tomcat.ConfigurableTomcatWebServerFactory
            + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
            + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
        + org.springframework.boot.web.embedded.undertow.ConfigurableUndertowWebServerFactory
            + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
            + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory

org.springframework.boot.web.server.ErrorPageRegistry
    + org.springframework.boot.web.servlet.support.ErrorPageFilter
    + org.springframework.boot.web.server.ConfigurableWebServerFactory
        + org.springframework.boot.web.server.AbstractConfigurableWebServerFactory
            + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
            + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.netty.NettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory
        + org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory
            + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
        + org.springframework.boot.web.reactive.server.ConfigurableReactiveWebServerFactory
            + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory
                + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.netty.NettyReactiveWebServerFactory
                + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
                + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory
        + org.springframework.boot.web.embedded.jetty.ConfigurableJettyWebServerFactory
            + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
            + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
        + org.springframework.boot.web.embedded.tomcat.ConfigurableTomcatWebServerFactory
            + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
            + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
        + org.springframework.boot.web.embedded.undertow.ConfigurableUndertowWebServerFactory
            + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory
            + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory

org.springframework.boot.web.servlet.server.ServletWebServerFactory
    + org.springframework.boot.web.servlet.server.ConfigurableServletWebServerFactory
        + org.springframework.boot.web.servlet.server.AbstractServletWebServerFactory
            + org.springframework.boot.web.embedded.jetty.JettyServletWebServerFactory
            + org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory
            + org.springframework.boot.web.embedded.undertow.UndertowServletWebServerFactory

org.springframework.boot.web.reactive.server.ReactiveWebServerFactory
    + org.springframework.boot.web.reactive.server.ConfigurableReactiveWebServerFactory
        + org.springframework.boot.web.reactive.server.AbstractReactiveWebServerFactory
            + org.springframework.boot.web.embedded.jetty.JettyReactiveWebServerFactory
            + org.springframework.boot.web.embedded.netty.NettyReactiveWebServerFactory
            + org.springframework.boot.web.embedded.tomcat.TomcatReactiveWebServerFactory
            + org.springframework.boot.web.embedded.undertow.UndertowReactiveWebServerFactory

org.springframework.boot.web.server.WebServerFactoryCustomizer<T>
    + org.springframework.boot.autoconfigure.web.embedded.JettyWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.embedded.NettyWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.embedded.TomcatWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.embedded.UndertowWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.servlet.TomcatServletWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.servlet.UndertowServletWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.reactive.ReactiveWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.web.reactive.TomcatReactiveWebServerFactoryCustomizer
    + org.springframework.boot.autoconfigure.websocket.servlet.JettyWebSocketServletWebServerCustomizer
    + org.springframework.boot.autoconfigure.websocket.servlet.TomcatWebSocketServletWebServerCustomizer
    + org.springframework.boot.autoconfigure.websocket.servlet.UndertowWebSocketServletWebServerCustomizer
    + org.springframework.boot.autoconfigure.websocket.reactive.TomcatWebSocketReactiveWebServerCustomizer
    + org.springframework.boot.actuate.autoconfigure.web.server.ManagementWebServerFactoryCustomizer<T>

org.springframework.boot.web.server.WebServerFactoryCustomizerBeanPostProcessor

org.springframework.boot.web.server.WebServer
    + org.springframework.boot.web.embedded.jetty.JettyWebServer
    + org.springframework.boot.web.embedded.netty.NettyWebServer
    + org.springframework.boot.web.embedded.tomcat.TomcatWebServer
    + org.springframework.boot.web.embedded.undertow.UndertowWebServer
        + org.springframework.boot.web.embedded.undertow.UndertowServletWebServer

org.springframework.boot.web.server.Http2
org.springframework.boot.web.server.Compression
org.springframework.boot.web.server.LocalServerPort
org.springframework.boot.web.server.MimeMappings
org.springframework.boot.web.server.MimeMappings.Mapping

org.springframework.boot.web.server.ErrorPage
org.springframework.boot.web.server.ErrorPageRegistrar
org.springframework.boot.web.server.ErrorPageRegistrarBeanPostProcessor

org.springframework.boot.web.server.Shutdown
org.springframework.boot.web.server.GracefulShutdownResult
org.springframework.boot.web.server.GracefulShutdownCallback

org.springframework.boot.web.server.Ssl
org.springframework.boot.web.server.Ssl.ClientAuth
org.springframework.boot.web.server.SslStoreProvider
org.springframework.boot.web.server.SslConfigurationValidator

org.springframework.boot.web.server.Cookie
    + org.springframework.boot.web.servlet.server.Session.Cookie

org.springframework.boot.web.server.Cookie.SameSite

org.springframework.boot.web.server.WebServerException
    + org.springframework.boot.web.server.PortInUseException
    + org.springframework.boot.web.embedded.tomcat.ConnectorStartFailedException

org.springframework.boot.web.embedded.jetty.JettyServerCustomizer
org.springframework.boot.web.embedded.jetty.ServletContextInitializerConfiguration

org.springframework.boot.web.embedded.netty.NettyRouteProvider

org.springframework.boot.web.embedded.netty.NettyServerCustomizer
    + org.springframework.boot.web.embedded.netty.SslServerCustomizer

org.springframework.boot.web.embedded.tomcat.TomcatEmbeddedWebappClassLoader
org.springframework.boot.web.embedded.tomcat.TomcatConnectorCustomizer
org.springframework.boot.web.embedded.tomcat.TomcatContextCustomizer
org.springframework.boot.web.embedded.tomcat.TomcatProtocolHandlerCustomizer

org.springframework.boot.web.embedded.undertow.HttpHandlerFactory
org.springframework.boot.web.embedded.undertow.UndertowBuilderCustomizer
org.springframework.boot.web.embedded.undertow.UndertowDeploymentInfoCustomizer
```

## logging

```java
org.springframework.boot.context.logging.LoggingApplicationListener
org.springframework.boot.logging.LoggingInitializationContext
org.springframework.boot.logging.LogFile
org.springframework.boot.logging.LogLevel
org.springframework.boot.logging.LoggerGroup
org.springframework.boot.logging.LoggerGroups
org.springframework.boot.logging.LoggerConfiguration

org.springframework.boot.logging.LoggingSystemFactory
    + org.springframework.boot.logging.java.JavaLoggingSystem.Factory
    + org.springframework.boot.logging.log4j2.Log4J2LoggingSystem.Factory
    + org.springframework.boot.logging.logback.LogbackLoggingSystem.Factory

org.springframework.boot.logging.LoggingSystem
    + org.springframework.boot.logging.AbstractLoggingSystem
        + org.springframework.boot.logging.java.JavaLoggingSystem
        + org.springframework.boot.logging.Slf4JLoggingSystem
            + org.springframework.boot.logging.log4j2.Log4J2LoggingSystem
            + org.springframework.boot.logging.logback.LogbackLoggingSystem

org.springframework.boot.logging.AbstractLoggingSystem.LogLevels

org.springframework.boot.logging.LoggingSystemProperties
    + org.springframework.boot.logging.logback.LogbackLoggingSystemProperties

org.springframework.boot.logging.DeferredLog

org.springframework.boot.logging.DeferredLogFactory
    + org.springframework.boot.logging.DeferredLogs

org.springframework.boot.logging.java.SimpleFormatter

org.springframework.boot.logging.log4j2.SpringBootConfigurationFactory
org.springframework.boot.logging.log4j2.SpringBootPropertySource
org.springframework.boot.logging.log4j2.ColorConverter
org.springframework.boot.logging.log4j2.WhitespaceThrowablePatternConverter
org.springframework.boot.logging.log4j2.ExtendedWhitespaceThrowablePatternConverter

org.springframework.boot.logging.logback.ColorConverter
org.springframework.boot.logging.logback.WhitespaceThrowableProxyConverter
org.springframework.boot.logging.logback.ExtendedWhitespaceThrowableProxyConverter
```

## admin

```java
org.springframework.boot.admin.SpringApplicationAdminMXBean
org.springframework.boot.admin.SpringApplicationAdminMXBeanRegistrar

org.springframework.boot.availability.AvailabilityChangeEvent

org.springframework.boot.availability.ApplicationAvailability
    + org.springframework.boot.availability.ApplicationAvailabilityBean

org.springframework.boot.availability.AvailabilityState
    + org.springframework.boot.availability.LivenessState
    + org.springframework.boot.availability.ReadinessState

org.springframework.boot.diagnostics.FailureAnalyzer
    + org.springframework.boot.diagnostics.AbstractFailureAnalyzer<T>
        + org.springframework.boot.diagnostics.analyzer.AbstractInjectionFailureAnalyzer<T>
            + org.springframework.boot.diagnostics.analyzer.BeanNotOfRequiredTypeFailureAnalyzer

org.springframework.boot.diagnostics.FailureAnalysisReporter
    + org.springframework.boot.diagnostics.LoggingFailureAnalysisReporter

org.springframework.boot.diagnostics.FailureAnalysis
```

## convert

```java
org.springframework.boot.convert.ApplicationConversionService
org.springframework.boot.convert.DataSizeUnit
org.springframework.boot.convert.Delimiter
org.springframework.boot.convert.DurationFormat
org.springframework.boot.convert.DurationStyle
org.springframework.boot.convert.DurationUnit
org.springframework.boot.convert.PeriodFormat
org.springframework.boot.convert.PeriodStyle
org.springframework.boot.convert.PeriodUnit
```

## EnvironmentPostProcessor

```java
org.springframework.boot.env.EnvironmentPostProcessor
    + org.springframework.boot.cloud.CloudFoundryVcapEnvironmentPostProcessor
    + org.springframework.boot.context.config.ConfigDataEnvironmentPostProcessor
    + org.springframework.boot.context.config.ConfigFileApplicationListener
    + org.springframework.boot.reactor.DebugAgentEnvironmentPostProcessor
    + org.springframework.boot.env.SpringApplicationJsonEnvironmentPostProcessor
    + org.springframework.boot.env.RandomValuePropertySourceEnvironmentPostProcessor
    + org.springframework.boot.env.SystemEnvironmentPropertySourceEnvironmentPostProcessor
    + org.springframework.boot.devtools.env.DevToolsHomePropertiesPostProcessor
    + org.springframework.boot.devtools.env.DevToolsPropertyDefaultsPostProcessor

org.springframework.boot.cloud.CloudPlatform
```

## properties

```java
org.springframework.boot.context.properties.EnableConfigurationProperties
org.springframework.boot.context.properties.ConfigurationPropertiesBinding
org.springframework.boot.context.properties.ConfigurationPropertiesScan
org.springframework.boot.context.properties.ConfigurationProperties
org.springframework.boot.context.properties.ConstructorBinding

org.springframework.boot.context.properties.source.ConfigurationPropertyName
org.springframework.boot.context.properties.source.ConfigurationPropertyName.Form
org.springframework.boot.context.properties.source.ConfigurationPropertyNameAliases
org.springframework.boot.context.properties.source.ConfigurationPropertyState
org.springframework.boot.context.properties.source.ConfigurationPropertyCaching

org.springframework.boot.context.properties.source.ConfigurationPropertySource
    + org.springframework.boot.context.properties.source.IterableConfigurationPropertySource
        + org.springframework.boot.context.properties.source.MapConfigurationPropertySource

org.springframework.boot.context.properties.source.ConfigurationPropertySources

org.springframework.boot.origin.Origin
    + org.springframework.boot.origin.PropertySourceOrigin
    + org.springframework.boot.origin.SystemEnvironmentOrigin
    + org.springframework.boot.origin.TextResourceOrigin

org.springframework.boot.origin.TextResourceOrigin.Location

org.springframework.boot.origin.OriginProvider
    + org.springframework.boot.origin.OriginTrackedValue
    + org.springframework.boot.context.config.ConfigDataLocation
    + org.springframework.boot.context.properties.bind.BindException
    + org.springframework.boot.context.properties.source.ConfigurationProperty
    + org.springframework.boot.origin.OriginTrackedResource
        + org.springframework.boot.origin.OriginTrackedResource.OriginTrackedWritableResource
    + org.springframework.boot.context.config.ConfigDataNotFoundException
        + org.springframework.boot.context.config.ConfigDataLocationNotFoundException
        + org.springframework.boot.context.config.ConfigDataResourceNotFoundException

org.springframework.boot.origin.OriginLookup
    + org.springframework.boot.env.ConfigTreePropertySource
    + org.springframework.boot.env.OriginTrackedMapPropertySource
    + org.springframework.boot.env.SystemEnvironmentPropertySourceEnvironmentPostProcessor.OriginAwareSystemEnvironmentPropertySource

org.springframework.boot.context.properties.BoundConfigurationProperties
org.springframework.boot.context.properties.ConfigurationPropertiesBean
org.springframework.boot.context.properties.ConfigurationPropertiesBean.BindMethod
org.springframework.boot.context.properties.ConfigurationPropertiesBindingPostProcessor
org.springframework.boot.context.properties.ConfigurationPropertiesBindHandlerAdvisor
org.springframework.boot.context.properties.ConfigurationPropertiesBindException

org.springframework.boot.context.properties.bind.BindHandler
    + org.springframework.boot.context.properties.bind.AbstractBindHandler
        + org.springframework.boot.context.properties.bind.BoundPropertiesTrackingBindHandler
        + org.springframework.boot.context.properties.bind.handler.IgnoreErrorsBindHandler
        + org.springframework.boot.context.properties.bind.handler.IgnoreTopLevelConverterNotFoundBindHandler
        + org.springframework.boot.context.properties.bind.handler.NoUnboundElementsBindHandler
        + org.springframework.boot.context.properties.bind.validation.ValidationBindHandler
```

## web

```java
org.springframework.boot.builder.ParentContextApplicationContextInitializer
org.springframework.boot.builder.ParentContextApplicationContextInitializer.ParentContextAvailableEvent
org.springframework.boot.context.ConfigurationWarningsApplicationContextInitializer
org.springframework.boot.context.ConfigurationWarningsApplicationContextInitializer.ConfigurationWarningsPostProcessor
org.springframework.boot.context.ContextIdApplicationContextInitializer
org.springframework.boot.context.config.DelegatingApplicationContextInitializer
org.springframework.boot.web.context.ServerPortInfoApplicationContextInitializer
org.springframework.boot.web.servlet.support.ServletContextApplicationContextInitializer
org.springframework.boot.rsocket.context.RSocketPortInfoApplicationContextInitializer
org.springframework.boot.autoconfigure.logging.ConditionEvaluationReportLoggingListener
org.springframework.boot.test.context.ConfigDataApplicationContextInitializer
org.springframework.boot.devtools.restart.RestartScopeInitializer

org.springframework.boot.context.ConfigurationWarningsApplicationContextInitializer.Check
    + org.springframework.boot.context.ConfigurationWarningsApplicationContextInitializer.ComponentScanPackageCheck

org.springframework.boot.web.context.WebServerApplicationContext
    + org.springframework.boot.web.context.ConfigurableWebServerApplicationContext
        + org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext
            + org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext
            + org.springframework.boot.web.servlet.context.XmlServletWebServerApplicationContext
        + org.springframework.boot.web.reactive.context.ReactiveWebServerApplicationContext
            + org.springframework.boot.web.reactive.context.AnnotationConfigReactiveWebServerApplicationContext

org.springframework.boot.web.servlet.context.AnnotationConfigServletWebApplicationContext
org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.ExistingWebApplicationScopes

org.springframework.boot.web.reactive.context.ReactiveWebApplicationContext
    + org.springframework.boot.web.reactive.context.ConfigurableReactiveWebApplicationContext
        + org.springframework.boot.web.reactive.context.AnnotationConfigReactiveWebApplicationContext
        + org.springframework.boot.test.context.assertj.AssertableReactiveWebApplicationContext
        + org.springframework.boot.web.reactive.context.GenericReactiveWebApplicationContext
            + org.springframework.boot.web.reactive.context.ReactiveWebServerApplicationContext
                + org.springframework.boot.web.reactive.context.AnnotationConfigReactiveWebServerApplicationContext

org.springframework.boot.web.context.WebServerInitializedEvent
    + org.springframework.boot.web.servlet.context.ServletWebServerInitializedEvent
    + org.springframework.boot.web.reactive.context.ReactiveWebServerInitializedEvent


org.springframework.boot.web.context.WebServerPortFileWriter
org.springframework.boot.web.context.WebServerGracefulShutdownLifecycle

org.springframework.boot.web.client.RestTemplateBuilder
org.springframework.boot.web.client.RestTemplateRequestCustomizer
org.springframework.boot.web.client.ClientHttpRequestFactorySupplier

org.springframework.boot.web.client.RestTemplateCustomizer
    + org.springframework.boot.actuate.metrics.web.client.MetricsRestTemplateCustomizer
    + org.springframework.boot.test.web.client.MockServerRestTemplateCustomizer

org.springframework.boot.web.client.RootUriTemplateHandler
    + org.springframework.boot.test.web.client.LocalHostUriTemplateHandler

org.springframework.boot.web.codec.CodecCustomizer

org.springframework.boot.web.error.ErrorAttributeOptions
org.springframework.boot.web.error.ErrorAttributeOptions.Include
```

## util

```java
org.springframework.boot.util.Instantiator
org.springframework.boot.util.Instantiator.AvailableParameters
org.springframework.boot.util.LambdaSafe
org.springframework.boot.util.LambdaSafe.InvocationResult

org.springframework.boot.util.LambdaSafe.LambdaSafeCallback
    + org.springframework.boot.util.LambdaSafe.Callback
    + org.springframework.boot.util.LambdaSafe.Callbacks
```

## webservices

```java
org.springframework.boot.webservices.client.HttpWebServiceMessageSenderBuilder
org.springframework.boot.webservices.client.WebServiceTemplateBuilder
org.springframework.boot.webservices.client.WebServiceTemplateCustomizer
```

## system

```java
org.springframework.boot.system.JavaVersion
org.springframework.boot.system.SystemProperties
org.springframework.boot.system.ApplicationPid
org.springframework.boot.system.ApplicationHome
org.springframework.boot.system.ApplicationTemp
```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

































































