

## AliasRegistry

```java
org.springframework.core.AliasRegistry
    + org.springframework.beans.factory.support.BeanDefinitionRegistry
        + org.springframework.beans.factory.support.DefaultListableBeanFactory
            + org.springframework.beans.factory.xml.XmlBeanFactory
        + org.springframework.context.support.GenericApplicationContext
            + org.springframework.context.annotation.AnnotationConfigApplicationContext
            + org.springframework.context.support.GenericGroovyApplicationContext
            + org.springframework.web.context.support.GenericWebApplicationContext
            + org.springframework.context.support.GenericXmlApplicationContext
            + org.springframework.jca.context.ResourceAdapterApplicationContext
            + org.springframework.context.support.StaticApplicationContext
                + org.springframework.web.context.support.StaticWebApplicationContext
        + org.springframework.beans.factory.support.SimpleBeanDefinitionRegistry
    + org.springframework.core.SimpleAliasRegistry
        + org.springframework.beans.factory.support.DefaultSingletonBeanRegistry
            + org.springframework.beans.factory.support.FactoryBeanRegistrySupport
                + org.springframework.beans.factory.support.AbstractBeanFactory
                    + org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory
                        + org.springframework.beans.factory.support.DefaultListableBeanFactory
                            + org.springframework.beans.factory.xml.XmlBeanFactory
        + org.springframework.beans.factory.support.SimpleBeanDefinitionRegistry
```

## AnnotationFilter

```java
org.springframework.core.annotation.AnnotationFilter
```

## MergedAnnotation

```java
org.springframework.core.annotation.MergedAnnotation
```

## MergedAnnotationSelector

```java
org.springframework.core.annotation.MergedAnnotationSelector
```

## SynthesizedAnnotation

```java
org.springframework.core.annotation.SynthesizedAnnotation
```

## AttributeAccessor

```java
org.springframework.core.AttributeAccessor
    + org.springframework.core.AttributeAccessorSupport
        + org.springframework.beans.BeanMetadataAttributeAccessor
            + org.springframework.beans.factory.support.AbstractBeanDefinition
                + org.springframework.beans.factory.support.ChildBeanDefinition
                + org.springframework.beans.factory.support.GenericBeanDefinition
                    + org.springframework.beans.factory.annotation.AnnotatedGenericBeanDefinition
                    + org.springframework.context.annotation.ScannedGenericBeanDefinition
                + org.springframework.beans.factory.support.RootBeanDefinition
            + org.springframework.beans.factory.support.AutowireCandidateQualifier
            + org.springframework.beans.PropertyValue
    + org.springframework.beans.factory.config.BeanDefinition
        + org.springframework.beans.factory.support.AbstractBeanDefinition
            + org.springframework.beans.factory.support.ChildBeanDefinition
            + org.springframework.beans.factory.support.GenericBeanDefinition
                + org.springframework.beans.factory.annotation.AnnotatedGenericBeanDefinition
                + org.springframework.context.annotation.ScannedGenericBeanDefinition
            + org.springframework.beans.factory.support.RootBeanDefinition
        + org.springframework.beans.factory.annotation.AnnotatedBeanDefinition
            + org.springframework.beans.factory.annotation.AnnotatedGenericBeanDefinition
            + org.springframework.context.annotation.ScannedGenericBeanDefinition
    + org.springframework.test.context.TestContext
        + org.springframework.test.context.support.DefaultTestContext
```

## Decoder

```java
org.springframework.core.codec.Decoder
    + org.springframework.core.codec.AbstractDecoder
        + org.springframework.core.codec.AbstractDataBufferDecoder
            + org.springframework.core.codec.ByteArrayDecoder
            + org.springframework.core.codec.ByteBufferDecoder
            + org.springframework.core.codec.DataBufferDecoder
            + org.springframework.core.codec.NettyByteBufDecoder
            + org.springframework.core.codec.ResourceDecoder
            + org.springframework.core.codec.StringDecoder
        + org.springframework.http.codec.xml.Jaxb2XmlDecoder
        + org.springframework.http.codec.json.KotlinSerializationJsonDecoder
        + org.springframework.http.codec.xml.XmlEventDecoder
    + org.springframework.http.codec.HttpMessageDecoder
        + org.springframework.http.codec.json.AbstractJackson2Decoder
            + org.springframework.http.codec.cbor.Jackson2CborDecoder
            + org.springframework.http.codec.json.Jackson2JsonDecoder
            + org.springframework.http.codec.json.Jackson2SmileDecoder
    + org.springframework.http.codec.protobuf.ProtobufDecoder
```

## Encoder

```java
org.springframework.core.codec.Encoder
    + org.springframework.core.codec.AbstractEncoder
        + org.springframework.core.codec.AbstractSingleValueEncoder
            + org.springframework.http.codec.xml.Jaxb2XmlEncoder
            + org.springframework.core.codec.ResourceEncoder
        + org.springframework.core.codec.ByteArrayEncoder
        + org.springframework.core.codec.ByteBufferEncoder
        + org.springframework.core.codec.CharSequenceEncoder
        + org.springframework.core.codec.DataBufferEncoder
        + org.springframework.http.codec.json.KotlinSerializationJsonEncoder
        + org.springframework.core.codec.NettyByteBufEncoder
        + org.springframework.core.codec.ResourceRegionEncoder
    + org.springframework.http.codec.HttpMessageEncoder
        + org.springframework.http.codec.json.AbstractJackson2Encoder
            + org.springframework.http.codec.cbor.Jackson2CborEncoder
            + org.springframework.http.codec.json.Jackson2JsonEncoder
            + org.springframework.http.codec.json.Jackson2SmileEncoder
        + org.springframework.http.codec.protobuf.ProtobufEncoder
```

## ConversionService

```java
org.springframework.core.convert.ConversionService
    + org.springframework.core.convert.support.ConfigurableConversionService
        + org.springframework.core.convert.support.GenericConversionService
            + org.springframework.core.convert.support.DefaultConversionService
            + org.springframework.format.support.FormattingConversionService
                + org.springframework.format.support.DefaultFormattingConversionService
```

## ConditionalConverter

```java
org.springframework.core.convert.converter.ConditionalConverter
    + org.springframework.core.convert.converter.ConditionalGenericConverter
```

## Converter

```java
org.springframework.core.convert.converter.Converter
    + org.springframework.core.serializer.support.DeserializingConverter
    + org.springframework.core.serializer.support.SerializingConverter
```

## ConverterFactory

```java
org.springframework.core.convert.converter.ConverterFactory
```

## ConverterRegistry

```java
org.springframework.core.convert.converter.ConverterRegistry
    + org.springframework.core.convert.support.ConfigurableConversionService
        + org.springframework.core.convert.support.GenericConversionService
            + org.springframework.core.convert.support.DefaultConversionService
            + org.springframework.format.support.FormattingConversionService
                + org.springframework.format.support.DefaultFormattingConversionService
    + org.springframework.format.FormatterRegistry
        + org.springframework.format.support.FormattingConversionService
            + org.springframework.format.support.DefaultFormattingConversionService
```

## GenericConverter

```java
org.springframework.core.convert.converter.GenericConverter
    + org.springframework.core.convert.converter.ConditionalGenericConverter
```

## DecoratingProxy

```java
org.springframework.core.DecoratingProxy
```

## EnvironmentCapable

```java
org.springframework.core.env.EnvironmentCapable
    + org.springframework.beans.factory.support.AbstractBeanDefinitionReader
        + org.springframework.beans.factory.groovy.GroovyBeanDefinitionReader
        + org.springframework.beans.factory.support.PropertiesBeanDefinitionReader
        + org.springframework.beans.factory.xml.XmlBeanDefinitionReader
    + org.springframework.context.ApplicationContext
        + org.springframework.context.ConfigurableApplicationContext
            + org.springframework.context.support.AbstractApplicationContext
                + org.springframework.context.support.AbstractRefreshableApplicationContext
                    + org.springframework.context.support.AbstractRefreshableConfigApplicationContext
                        + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                            + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                            + org.springframework.web.context.support.GroovyWebApplicationContext
                            + org.springframework.web.context.support.XmlWebApplicationContext
                        + org.springframework.context.support.AbstractXmlApplicationContext
                            + org.springframework.context.support.ClassPathXmlApplicationContext
                            + org.springframework.context.support.FileSystemXmlApplicationContext
                + org.springframework.context.support.GenericApplicationContext
                    + org.springframework.context.annotation.AnnotationConfigApplicationContext
                    + org.springframework.context.support.GenericGroovyApplicationContext
                    + org.springframework.web.context.support.GenericWebApplicationContext
                    + org.springframework.context.support.GenericXmlApplicationContext
                    + org.springframework.jca.context.ResourceAdapterApplicationContext
                    + org.springframework.context.support.StaticApplicationContext
                        + org.springframework.web.context.support.StaticWebApplicationContext
            + org.springframework.web.context.ConfigurableWebApplicationContext
                + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                    + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                    + org.springframework.web.context.support.GroovyWebApplicationContext
                    + org.springframework.web.context.support.XmlWebApplicationContext
                + org.springframework.web.context.support.GenericWebApplicationContext
                + org.springframework.web.context.support.StaticWebApplicationContext
        + org.springframework.web.context.WebApplicationContext
            + org.springframework.web.context.ConfigurableWebApplicationContext
                + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                    + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                    + org.springframework.web.context.support.GroovyWebApplicationContext
                    + org.springframework.web.context.support.XmlWebApplicationContext
                + org.springframework.web.context.support.GenericWebApplicationContext
                + org.springframework.web.context.support.StaticWebApplicationContext
    + org.springframework.context.annotation.ClassPathScanningCandidateComponentProvider
        + org.springframework.context.annotation.ClassPathBeanDefinitionScanner
    + org.springframework.web.filter.GenericFilterBean
        + org.springframework.web.filter.DelegatingFilterProxy
        + org.springframework.web.filter.OncePerRequestFilter
            + org.springframework.web.filter.AbstractRequestLoggingFilter
                + org.springframework.web.filter.CommonsRequestLoggingFilter
                + org.springframework.web.filter.ServletContextRequestLoggingFilter
            + org.springframework.web.filter.CharacterEncodingFilter
            + org.springframework.web.filter.CorsFilter
            + org.springframework.web.filter.FormContentFilter
            + org.springframework.web.filter.ForwardedHeaderFilter
            + org.springframework.web.filter.HiddenHttpMethodFilter
            + org.springframework.web.filter.HttpPutFormContentFilter
            + org.springframework.web.multipart.support.MultipartFilter
            + org.springframework.orm.jpa.support.OpenEntityManagerInViewFilter
            + org.springframework.orm.hibernate5.support.OpenSessionInViewFilter
            + org.springframework.web.filter.RelativeRedirectFilter
            + org.springframework.web.filter.RequestContextFilter
            + org.springframework.web.filter.ShallowEtagHeaderFilter
        + org.springframework.web.servlet.resource.ResourceUrlEncodingFilter
    + org.springframework.web.servlet.HttpServletBean
        + org.springframework.web.servlet.FrameworkServlet
            + org.springframework.web.servlet.DispatcherServlet
```

## Profiles

```java
org.springframework.core.env.Profiles
```

## PropertyResolver

```java
org.springframework.core.env.PropertyResolver
    + org.springframework.core.env.ConfigurablePropertyResolver
        + org.springframework.core.env.AbstractPropertyResolver
            + org.springframework.core.env.PropertySourcesPropertyResolver
        + org.springframework.core.env.ConfigurableEnvironment
            + org.springframework.core.env.AbstractEnvironment
                + org.springframework.mock.env.MockEnvironment
                + org.springframework.core.env.StandardEnvironment
                    + org.springframework.web.context.support.StandardServletEnvironment
            + org.springframework.web.context.ConfigurableWebEnvironment
                + org.springframework.web.context.support.StandardServletEnvironment
    + org.springframework.core.env.Environment
        + org.springframework.core.env.ConfigurableEnvironment
            + org.springframework.core.env.AbstractEnvironment
                + org.springframework.mock.env.MockEnvironment
                + org.springframework.core.env.StandardEnvironment
                    + org.springframework.web.context.support.StandardServletEnvironment
            + org.springframework.web.context.ConfigurableWebEnvironment
                + org.springframework.web.context.support.StandardServletEnvironment
```

## InfrastructureProxy

```java
org.springframework.core.InfrastructureProxy
```

## DataBuffer

```java
org.springframework.core.io.buffer.DataBuffer
    + org.springframework.core.io.buffer.DataBufferWrapper
    + org.springframework.core.io.buffer.DefaultDataBuffer
    + org.springframework.core.io.buffer.PooledDataBuffer
        + org.springframework.core.io.buffer.NettyDataBuffer
```

## DataBufferFactory

```java
org.springframework.core.io.buffer.DataBufferFactory
    + org.springframework.core.io.buffer.DefaultDataBufferFactory
    + org.springframework.core.io.buffer.NettyDataBufferFactory
```

## Matcher

```java
org.springframework.core.io.buffer.DataBufferUtils.Matcher
```

## InputStreamSource

```java
org.springframework.core.io.InputStreamSource
    + org.springframework.core.io.support.EncodedResource
    + org.springframework.web.multipart.MultipartFile
        + org.springframework.web.multipart.commons.CommonsMultipartFile
        + org.springframework.mock.web.MockMultipartFile
    + org.springframework.core.io.Resource
        + org.springframework.core.io.AbstractResource
            + org.springframework.core.io.AbstractFileResolvingResource
                + org.springframework.core.io.ClassPathResource
                    + org.springframework.core.io.DefaultResourceLoader.ClassPathContextResource
                + org.springframework.web.context.support.ServletContextResource
                + org.springframework.core.io.UrlResource
                    + org.springframework.core.io.FileUrlResource
            + org.springframework.core.io.ByteArrayResource
                + org.springframework.web.reactive.resource.TransformedResource
                + org.springframework.web.servlet.resource.TransformedResource
            + org.springframework.core.io.DescriptiveResource
            + org.springframework.core.io.FileSystemResource
            + org.springframework.core.io.InputStreamResource
            + org.springframework.core.io.PathResource
            + org.springframework.core.io.VfsResource
        + org.springframework.core.io.ContextResource
            + org.springframework.core.io.DefaultResourceLoader.ClassPathContextResource
            + org.springframework.web.context.support.ServletContextResource
        + org.springframework.web.reactive.resource.HttpResource
        + org.springframework.web.servlet.resource.HttpResource
        + org.springframework.core.io.WritableResource
            + org.springframework.core.io.FileSystemResource
            + org.springframework.core.io.FileUrlResource
            + org.springframework.core.io.PathResource
```

## ProtocolResolver

```java
org.springframework.core.io.ProtocolResolver
```

## ResourceLoader

```java
org.springframework.core.io.ResourceLoader
    + org.springframework.core.io.DefaultResourceLoader
        + org.springframework.context.support.AbstractApplicationContext
            + org.springframework.context.support.AbstractRefreshableApplicationContext
                + org.springframework.context.support.AbstractRefreshableConfigApplicationContext
                    + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                        + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                        + org.springframework.web.context.support.GroovyWebApplicationContext
                        + org.springframework.web.context.support.XmlWebApplicationContext
                    + org.springframework.context.support.AbstractXmlApplicationContext
                        + org.springframework.context.support.ClassPathXmlApplicationContext
                        + org.springframework.context.support.FileSystemXmlApplicationContext
            + org.springframework.context.support.GenericApplicationContext
                + org.springframework.context.annotation.AnnotationConfigApplicationContext
                + org.springframework.context.support.GenericGroovyApplicationContext
                + org.springframework.web.context.support.GenericWebApplicationContext
                + org.springframework.context.support.GenericXmlApplicationContext
                + org.springframework.jca.context.ResourceAdapterApplicationContext
                + org.springframework.context.support.StaticApplicationContext
                    + org.springframework.web.context.support.StaticWebApplicationContext
        + org.springframework.core.io.ClassRelativeResourceLoader
        + org.springframework.core.io.FileSystemResourceLoader
        + org.springframework.web.context.support.ServletContextResourceLoader
    + org.springframework.core.io.support.ResourcePatternResolver
        + org.springframework.context.ApplicationContext
            + org.springframework.context.ConfigurableApplicationContext
                + org.springframework.context.support.AbstractApplicationContext
                    + org.springframework.context.support.AbstractRefreshableApplicationContext
                        + org.springframework.context.support.AbstractRefreshableConfigApplicationContext
                            + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                                + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                                + org.springframework.web.context.support.GroovyWebApplicationContext
                                + org.springframework.web.context.support.XmlWebApplicationContext
                            + org.springframework.context.support.AbstractXmlApplicationContext
                                + org.springframework.context.support.ClassPathXmlApplicationContext
                                + org.springframework.context.support.FileSystemXmlApplicationContext
                    + org.springframework.context.support.GenericApplicationContext
                        + org.springframework.context.annotation.AnnotationConfigApplicationContext
                        + org.springframework.context.support.GenericGroovyApplicationContext
                        + org.springframework.web.context.support.GenericWebApplicationContext
                        + org.springframework.context.support.GenericXmlApplicationContext
                        + org.springframework.jca.context.ResourceAdapterApplicationContext
                        + org.springframework.context.support.StaticApplicationContext
                            + org.springframework.web.context.support.StaticWebApplicationContext
                + org.springframework.web.context.ConfigurableWebApplicationContext
                    + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                        + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                        + org.springframework.web.context.support.GroovyWebApplicationContext
                        + org.springframework.web.context.support.XmlWebApplicationContext
                    + org.springframework.web.context.support.GenericWebApplicationContext
                    + org.springframework.web.context.support.StaticWebApplicationContext
            + org.springframework.web.context.WebApplicationContext
                + org.springframework.web.context.ConfigurableWebApplicationContext
                    + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
                        + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
                        + org.springframework.web.context.support.GroovyWebApplicationContext
                        + org.springframework.web.context.support.XmlWebApplicationContext
                    + org.springframework.web.context.support.GenericWebApplicationContext
                    + org.springframework.web.context.support.StaticWebApplicationContext
        + org.springframework.core.io.support.PathMatchingResourcePatternResolver
            + org.springframework.web.context.support.ServletContextResourcePatternResolver
```

## PropertySourceFactory

```java
org.springframework.core.io.support.PropertySourceFactory
    + org.springframework.core.io.support.DefaultPropertySourceFactory
```

## MetadataLookup

```java
org.springframework.core.MethodIntrospector.MetadataLookup
```

## ApplicationStartup

```java
org.springframework.core.metrics.ApplicationStartup
    + org.springframework.core.metrics.jfr.FlightRecorderApplicationStartup
```

## StartupStep

```java
org.springframework.core.metrics.StartupStep
```

## Tag

```java
org.springframework.core.metrics.StartupStep.Tag
```

## OrderSourceProvider

```java
org.springframework.core.OrderComparator.OrderSourceProvider
```

## Ordered

```java
org.springframework.core.Ordered
    + org.springframework.web.servlet.handler.AbstractHandlerExceptionResolver
        + org.springframework.web.servlet.handler.AbstractHandlerMethodExceptionResolver
            + org.springframework.web.servlet.mvc.method.annotation.ExceptionHandlerExceptionResolver
        + org.springframework.web.servlet.mvc.support.DefaultHandlerExceptionResolver
        + org.springframework.web.servlet.mvc.annotation.ResponseStatusExceptionResolver
        + org.springframework.web.servlet.handler.SimpleMappingExceptionResolver
    + org.springframework.web.reactive.handler.AbstractHandlerMapping
        + org.springframework.web.reactive.result.method.AbstractHandlerMethodMapping
            + org.springframework.web.reactive.result.method.RequestMappingInfoHandlerMapping
                + org.springframework.web.reactive.result.method.annotation.RequestMappingHandlerMapping
        + org.springframework.web.reactive.handler.AbstractUrlHandlerMapping
            + org.springframework.web.reactive.handler.SimpleUrlHandlerMapping
        + org.springframework.web.reactive.function.server.support.RouterFunctionMapping
    + org.springframework.web.servlet.handler.AbstractHandlerMapping
        + org.springframework.web.servlet.handler.AbstractHandlerMethodMapping
            + org.springframework.web.servlet.mvc.method.RequestMappingInfoHandlerMapping
                + org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping
        + org.springframework.web.servlet.handler.AbstractUrlHandlerMapping
            + org.springframework.web.servlet.handler.AbstractDetectingUrlHandlerMapping
                + org.springframework.web.servlet.handler.BeanNameUrlHandlerMapping
            + org.springframework.web.servlet.handler.SimpleUrlHandlerMapping
                + org.springframework.web.socket.server.support.WebSocketHandlerMapping
        + org.springframework.web.servlet.function.support.RouterFunctionMapping
    + org.springframework.web.servlet.mvc.method.AbstractHandlerMethodAdapter
        + org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter
    + org.springframework.aop.support.AbstractPointcutAdvisor
        + org.springframework.aop.support.AbstractBeanFactoryPointcutAdvisor
            + org.springframework.cache.interceptor.BeanFactoryCacheOperationSourceAdvisor
            + org.springframework.cache.jcache.interceptor.BeanFactoryJCacheOperationSourceAdvisor
            + org.springframework.transaction.interceptor.BeanFactoryTransactionAttributeSourceAdvisor
            + org.springframework.aop.support.DefaultBeanFactoryPointcutAdvisor
        + org.springframework.aop.support.AbstractGenericPointcutAdvisor
            + org.springframework.aop.aspectj.AspectJExpressionPointcutAdvisor
            + org.springframework.aop.support.DefaultPointcutAdvisor
                + org.springframework.aop.aspectj.annotation.ReflectiveAspectJAdvisorFactory.SyntheticInstantiationAdvisor
            + org.springframework.aop.support.NameMatchMethodPointcutAdvisor
            + org.springframework.aop.support.RegexpMethodPointcutAdvisor
        + org.springframework.scheduling.annotation.AsyncAnnotationAdvisor
        + org.springframework.dao.annotation.PersistenceExceptionTranslationAdvisor
        + org.springframework.transaction.interceptor.TransactionAttributeSourceAdvisor
    + org.springframework.test.context.support.AbstractTestExecutionListener
        + org.springframework.test.context.support.AbstractDirtiesContextTestExecutionListener
            + org.springframework.test.context.support.DirtiesContextBeforeModesTestExecutionListener
            + org.springframework.test.context.support.DirtiesContextTestExecutionListener
        + org.springframework.test.context.event.ApplicationEventsTestExecutionListener
        + org.springframework.test.context.support.DependencyInjectionTestExecutionListener
        + org.springframework.test.context.event.EventPublishingTestExecutionListener
        + org.springframework.test.context.web.ServletTestExecutionListener
        + org.springframework.test.context.jdbc.SqlScriptsTestExecutionListener
        + org.springframework.test.context.transaction.TransactionalTestExecutionListener
    + org.springframework.aop.aspectj.AspectInstanceFactory
        + org.springframework.aop.aspectj.annotation.MetadataAwareAspectInstanceFactory
            + org.springframework.aop.aspectj.annotation.BeanFactoryAspectInstanceFactory
                + org.springframework.aop.aspectj.annotation.PrototypeAspectInstanceFactory
            + org.springframework.aop.aspectj.annotation.LazySingletonAspectInstanceFactoryDecorator
            + org.springframework.aop.aspectj.annotation.SimpleMetadataAwareAspectInstanceFactory
            + org.springframework.aop.aspectj.annotation.SingletonMetadataAwareAspectInstanceFactory
        + org.springframework.aop.aspectj.SimpleAspectInstanceFactory
            + org.springframework.aop.aspectj.annotation.SimpleMetadataAwareAspectInstanceFactory
        + org.springframework.aop.config.SimpleBeanFactoryAwareAspectInstanceFactory
        + org.springframework.aop.aspectj.SingletonAspectInstanceFactory
            + org.springframework.aop.aspectj.annotation.SingletonMetadataAwareAspectInstanceFactory
    + org.springframework.aop.aspectj.AspectJPointcutAdvisor
    + org.springframework.aop.aspectj.AspectJPrecedenceInformation
        + org.springframework.aop.aspectj.AbstractAspectJAdvice
            + org.springframework.aop.aspectj.AspectJAfterAdvice
            + org.springframework.aop.aspectj.AspectJAfterReturningAdvice
            + org.springframework.aop.aspectj.AspectJAfterThrowingAdvice
            + org.springframework.aop.aspectj.AspectJAroundAdvice
            + org.springframework.aop.aspectj.AspectJMethodBeforeAdvice
    + org.springframework.context.weaving.AspectJWeavingEnabler
    + org.springframework.aop.interceptor.AsyncExecutionInterceptor
        + org.springframework.scheduling.annotation.AnnotationAsyncExecutionInterceptor
    + org.springframework.web.servlet.view.BeanNameViewResolver
    + org.springframework.web.servlet.view.ContentNegotiatingViewResolver
    + org.springframework.web.method.ControllerAdviceBean
    + org.springframework.beans.factory.annotation.CustomAutowireConfigurer
    + org.springframework.beans.factory.config.CustomEditorConfigurer
    + org.springframework.beans.factory.config.CustomScopeConfigurer
    + org.springframework.context.event.DefaultEventListenerFactory
    + org.springframework.aop.support.DefaultIntroductionAdvisor
    + org.springframework.beans.ExtendedBeanInfoFactory
    + org.springframework.web.servlet.handler.HandlerExceptionResolverComposite
    + org.springframework.web.servlet.function.support.HandlerFunctionAdapter
    + org.springframework.web.reactive.result.HandlerResultHandlerSupport
        + org.springframework.web.reactive.result.method.annotation.AbstractMessageWriterResultHandler
            + org.springframework.web.reactive.result.method.annotation.ResponseBodyResultHandler
            + org.springframework.web.reactive.result.method.annotation.ResponseEntityResultHandler
        + org.springframework.web.reactive.result.view.ViewResolutionResultHandler
    + org.springframework.jms.annotation.JmsListenerAnnotationBeanPostProcessor
    + org.springframework.messaging.handler.MessagingAdviceBean
    + org.springframework.core.PriorityOrdered
        + org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor
        + org.springframework.context.annotation.ConfigurationClassPostProcessor
        + org.springframework.aop.interceptor.ExposeInvocationInterceptor
        + org.springframework.beans.factory.annotation.InitDestroyAnnotationBeanPostProcessor
            + org.springframework.context.annotation.CommonAnnotationBeanPostProcessor
        + org.springframework.orm.jpa.support.PersistenceAnnotationBeanPostProcessor
        + org.springframework.beans.factory.config.PropertyResourceConfigurer
            + org.springframework.beans.factory.config.PlaceholderConfigurerSupport
                + org.springframework.beans.factory.config.PropertyPlaceholderConfigurer
                    + org.springframework.beans.factory.config.PreferencesPlaceholderConfigurer
                + org.springframework.context.support.PropertySourcesPlaceholderConfigurer
            + org.springframework.beans.factory.config.PropertyOverrideConfigurer
        + org.springframework.beans.factory.annotation.RequiredAnnotationBeanPostProcessor
    + org.springframework.aop.framework.ProxyProcessorSupport
        + org.springframework.aop.framework.AbstractAdvisingBeanPostProcessor
            + org.springframework.aop.framework.autoproxy.AbstractBeanFactoryAwareAdvisingPostProcessor
                + org.springframework.scheduling.annotation.AsyncAnnotationBeanPostProcessor
                + org.springframework.validation.beanvalidation.MethodValidationPostProcessor
                + org.springframework.dao.annotation.PersistenceExceptionTranslationPostProcessor
        + org.springframework.aop.framework.autoproxy.AbstractAutoProxyCreator
            + org.springframework.aop.framework.autoproxy.AbstractAdvisorAutoProxyCreator
                + org.springframework.aop.aspectj.autoproxy.AspectJAwareAdvisorAutoProxyCreator
                    + org.springframework.aop.aspectj.annotation.AnnotationAwareAspectJAutoProxyCreator
                + org.springframework.aop.framework.autoproxy.DefaultAdvisorAutoProxyCreator
                + org.springframework.aop.framework.autoproxy.InfrastructureAdvisorAutoProxyCreator
            + org.springframework.aop.framework.autoproxy.BeanNameAutoProxyCreator
    + org.springframework.web.servlet.view.ResourceBundleViewResolver
    + org.springframework.scheduling.annotation.ScheduledAnnotationBeanPostProcessor
    + org.springframework.scripting.support.ScriptFactoryPostProcessor
    + org.springframework.web.reactive.function.server.support.ServerResponseResultHandler
    + org.springframework.context.event.SmartApplicationListener
        + org.springframework.web.socket.messaging.DefaultSimpUserRegistry
        + org.springframework.context.event.GenericApplicationListener
            + org.springframework.context.event.ApplicationListenerMethodAdapter
                + org.springframework.transaction.event.TransactionalApplicationListenerMethodAdapter
            + org.springframework.context.event.GenericApplicationListenerAdapter
            + org.springframework.context.event.SourceFilteringListener
        + org.springframework.messaging.simp.user.MultiServerUserRegistry
    + org.springframework.orm.hibernate5.SpringSessionSynchronization
    + org.springframework.aop.support.StaticMethodMatcherPointcutAdvisor
    + org.springframework.transaction.support.TransactionSynchronization
        + org.springframework.transaction.support.ResourceHolderSynchronization
        + org.springframework.orm.hibernate5.SpringFlushSynchronization
        + org.springframework.orm.hibernate5.SpringSessionSynchronization
        + org.springframework.transaction.support.TransactionSynchronizationAdapter
    + org.springframework.transaction.support.TransactionSynchronizationAdapter
    + org.springframework.transaction.event.TransactionalApplicationListener
        + org.springframework.transaction.event.TransactionalApplicationListenerAdapter
        + org.springframework.transaction.event.TransactionalApplicationListenerMethodAdapter
    + org.springframework.transaction.event.TransactionalApplicationListenerAdapter
    + org.springframework.transaction.event.TransactionalEventListenerFactory
    + org.springframework.web.servlet.view.UrlBasedViewResolver
        + org.springframework.web.servlet.view.AbstractTemplateViewResolver
            + org.springframework.web.servlet.view.freemarker.FreeMarkerViewResolver
            + org.springframework.web.servlet.view.groovy.GroovyMarkupViewResolver
        + org.springframework.web.servlet.view.InternalResourceViewResolver
        + org.springframework.web.servlet.view.script.ScriptTemplateViewResolver
        + org.springframework.web.servlet.view.tiles3.TilesViewResolver
        + org.springframework.web.servlet.view.xslt.XsltViewResolver
    + org.springframework.web.reactive.result.view.ViewResolutionResultHandler
    + org.springframework.web.servlet.view.ViewResolverComposite
    + org.springframework.web.reactive.result.view.ViewResolverSupport
        + org.springframework.web.reactive.result.view.UrlBasedViewResolver
            + org.springframework.web.reactive.result.view.freemarker.FreeMarkerViewResolver
            + org.springframework.web.reactive.result.view.script.ScriptTemplateViewResolver
    + org.springframework.web.reactive.socket.server.support.WebSocketHandlerAdapter
    + org.springframework.web.servlet.view.XmlViewResolver
```

## ParameterNameDiscoverer

```java
org.springframework.core.ParameterNameDiscoverer
    + org.springframework.aop.aspectj.AspectJAdviceParameterNameDiscoverer
    + org.springframework.core.KotlinReflectionParameterNameDiscoverer
    + org.springframework.core.LocalVariableTableParameterNameDiscoverer
    + org.springframework.core.PrioritizedParameterNameDiscoverer
        + org.springframework.core.DefaultParameterNameDiscoverer
    + org.springframework.core.StandardReflectionParameterNameDiscoverer
```

## ResolvableTypeProvider

```java
org.springframework.core.ResolvableTypeProvider
    + org.springframework.context.PayloadApplicationEvent
```

## Deserializer

```java
org.springframework.core.serializer.Deserializer
    + org.springframework.core.serializer.DefaultDeserializer
    + org.springframework.core.serializer.support.SerializationDelegate
```

## Serializer

```java
org.springframework.core.serializer.Serializer
    + org.springframework.core.serializer.DefaultSerializer
    + org.springframework.core.serializer.support.SerializationDelegate
```

## SmartClassLoader

```java
org.springframework.core.SmartClassLoader
```

## ToStringStyler

```java
org.springframework.core.style.ToStringStyler
    + org.springframework.core.style.DefaultToStringStyler
```

## ValueStyler

```java
org.springframework.core.style.ValueStyler
    + org.springframework.core.style.DefaultValueStyler
```

## TaskDecorator

```java
org.springframework.core.task.TaskDecorator
```

## AnnotatedTypeMetadata

```java
org.springframework.core.type.AnnotatedTypeMetadata
    + org.springframework.core.type.AnnotationMetadata
        + org.springframework.core.type.classreading.AnnotationMetadataReadingVisitor
        + org.springframework.core.type.StandardAnnotationMetadata
    + org.springframework.core.type.MethodMetadata
        + org.springframework.core.type.classreading.MethodMetadataReadingVisitor
        + org.springframework.core.type.StandardMethodMetadata
```

## ClassMetadata

```java
org.springframework.core.type.ClassMetadata
    + org.springframework.core.type.AnnotationMetadata
        + org.springframework.core.type.classreading.AnnotationMetadataReadingVisitor
        + org.springframework.core.type.StandardAnnotationMetadata
    + org.springframework.core.type.StandardClassMetadata
        + org.springframework.core.type.StandardAnnotationMetadata
```

## MetadataReader

```java
org.springframework.core.type.classreading.MetadataReader
```

## MetadataReaderFactory

```java
org.springframework.core.type.classreading.MetadataReaderFactory
    + org.springframework.core.type.classreading.SimpleMetadataReaderFactory
        + org.springframework.core.type.classreading.CachingMetadataReaderFactory
```

## TypeFilter

```java
org.springframework.core.type.filter.TypeFilter
    + org.springframework.core.type.filter.AbstractClassTestingTypeFilter
        + org.springframework.core.type.filter.RegexPatternTypeFilter
    + org.springframework.core.type.filter.AbstractTypeHierarchyTraversingFilter
        + org.springframework.core.type.filter.AnnotationTypeFilter
        + org.springframework.core.type.filter.AssignableTypeFilter
    + org.springframework.core.type.filter.AspectJTypeFilter
```