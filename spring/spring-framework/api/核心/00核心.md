
## org.springframework.core.AliasRegistry

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

## org.springframework.core.annotation.AliasFor

```java
org.springframework.core.annotation.AliasFor
```

## org.springframework.core.annotation.AnnotatedElementUtils

```java
org.springframework.core.annotation.AnnotatedElementUtils
```

## org.springframework.core.annotation.AnnotationAttributes

```java
org.springframework.core.annotation.AnnotationAttributes
```

## org.springframework.core.annotation.AnnotationFilter

```java
org.springframework.core.annotation.AnnotationFilter
```

## org.springframework.core.annotation.AnnotationUtils

```java
org.springframework.core.annotation.AnnotationUtils
```

## org.springframework.core.annotation.MergedAnnotation

```java
org.springframework.core.annotation.MergedAnnotation
```

## org.springframework.core.annotation.MergedAnnotation.Adapt

```java
org.springframework.core.annotation.MergedAnnotation.Adapt
```

## org.springframework.core.annotation.MergedAnnotationCollectors

```java
org.springframework.core.annotation.MergedAnnotationCollectors
```

## org.springframework.core.annotation.MergedAnnotationPredicates

```java
org.springframework.core.annotation.MergedAnnotationPredicates
```

## org.springframework.core.annotation.MergedAnnotations

```java
org.springframework.core.annotation.MergedAnnotations
```

## org.springframework.core.annotation.MergedAnnotations.SearchStrategy

```java
org.springframework.core.annotation.MergedAnnotations.SearchStrategy
```

## org.springframework.core.annotation.MergedAnnotationSelector

```java
org.springframework.core.annotation.MergedAnnotationSelector
```

## org.springframework.core.annotation.MergedAnnotationSelectors

```java
org.springframework.core.annotation.MergedAnnotationSelectors
```

## org.springframework.core.annotation.Order

```java
org.springframework.core.annotation.Order
```

## org.springframework.core.annotation.OrderUtils

```java
org.springframework.core.annotation.OrderUtils
```

## org.springframework.core.annotation.RepeatableContainers

```java
org.springframework.core.annotation.RepeatableContainers
```

## org.springframework.core.annotation.SynthesizedAnnotation

```java
org.springframework.core.annotation.SynthesizedAnnotation
```

## org.springframework.core.AttributeAccessor

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

## org.springframework.core.BridgeMethodResolver

```java
org.springframework.core.BridgeMethodResolver
```

## org.springframework.core.codec.Decoder

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

## org.springframework.core.codec.Encoder

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

## org.springframework.core.codec.Hints

```java
org.springframework.core.codec.Hints
```

## org.springframework.core.CollectionFactory

```java
org.springframework.core.CollectionFactory
```

## org.springframework.core.ConfigurableObjectInputStream

```java
org.springframework.core.ConfigurableObjectInputStream
    + org.springframework.remoting.rmi.CodebaseAwareObjectInputStream
```

## org.springframework.core.Constants

```java
org.springframework.core.Constants
```

## org.springframework.core.Constants.ConstantException

```java
org.springframework.core.Constants.ConstantException
```

## org.springframework.core.Conventions

```java
org.springframework.core.Conventions
```

## org.springframework.core.convert.ConversionService

```java
org.springframework.core.convert.ConversionService
    + org.springframework.core.convert.support.ConfigurableConversionService
        + org.springframework.core.convert.support.GenericConversionService
            + org.springframework.core.convert.support.DefaultConversionService
            + org.springframework.format.support.FormattingConversionService
                + org.springframework.format.support.DefaultFormattingConversionService
```

## org.springframework.core.convert.converter.ConditionalConverter

```java
org.springframework.core.convert.converter.ConditionalConverter
    + org.springframework.core.convert.converter.ConditionalGenericConverter
```

## org.springframework.core.convert.converter.Converter

```java
org.springframework.core.convert.converter.Converter
    + org.springframework.core.serializer.support.DeserializingConverter
    + org.springframework.core.serializer.support.SerializingConverter
```

## org.springframework.core.convert.converter.ConverterFactory

```java
org.springframework.core.convert.converter.ConverterFactory
```

## org.springframework.core.convert.converter.ConverterRegistry

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

## org.springframework.core.convert.converter.ConvertingComparator

```java
org.springframework.core.convert.converter.ConvertingComparator
```

## org.springframework.core.convert.converter.GenericConverter

```java
org.springframework.core.convert.converter.GenericConverter
    + org.springframework.core.convert.converter.ConditionalGenericConverter
```

## org.springframework.core.convert.converter.GenericConverter.ConvertiblePair

```java
org.springframework.core.convert.converter.GenericConverter.ConvertiblePair
```

## org.springframework.core.convert.Property

```java
org.springframework.core.convert.Property
```

## org.springframework.core.convert.support.ConversionServiceFactory

```java
org.springframework.core.convert.support.ConversionServiceFactory
```

## org.springframework.core.convert.support.ConvertingPropertyEditorAdapter

```java
org.springframework.core.convert.support.ConvertingPropertyEditorAdapter
```

## org.springframework.core.convert.TypeDescriptor

```java
org.springframework.core.convert.TypeDescriptor
```

## org.springframework.core.CoroutinesUtils

```java
org.springframework.core.CoroutinesUtils
```

## org.springframework.core.DecoratingClassLoader

```java
org.springframework.core.DecoratingClassLoader
    + org.springframework.core.OverridingClassLoader
        + org.springframework.instrument.classloading.SimpleInstrumentableClassLoader
        + org.springframework.instrument.classloading.SimpleThrowawayClassLoader
    + org.springframework.instrument.classloading.ShadowingClassLoader
        + org.springframework.instrument.classloading.ResourceOverridingShadowingClassLoader
```

## org.springframework.core.DecoratingProxy

```java
org.springframework.core.DecoratingProxy
```

## org.springframework.core.env.EnvironmentCapable

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

## org.springframework.core.env.MissingRequiredPropertiesException

```java
org.springframework.core.env.MissingRequiredPropertiesException
```

## org.springframework.core.env.Profiles

```java
org.springframework.core.env.Profiles
```

## org.springframework.core.env.PropertyResolver

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

## org.springframework.core.env.PropertySource

```java
org.springframework.core.env.PropertySource
    + org.springframework.core.env.EnumerablePropertySource
        + org.springframework.core.env.CommandLinePropertySource
            + org.springframework.core.env.JOptCommandLinePropertySource
            + org.springframework.core.env.SimpleCommandLinePropertySource
        + org.springframework.core.env.CompositePropertySource
        + org.springframework.core.env.MapPropertySource
            + org.springframework.core.env.PropertiesPropertySource
                + org.springframework.mock.env.MockPropertySource
                + org.springframework.core.io.support.ResourcePropertySource
            + org.springframework.core.env.SystemEnvironmentPropertySource
        + org.springframework.web.context.support.ServletConfigPropertySource
        + org.springframework.web.context.support.ServletContextPropertySource
    + org.springframework.jndi.JndiPropertySource
    + org.springframework.core.env.PropertySource.StubPropertySource
```

## org.springframework.core.env.PropertySources

```java
org.springframework.core.env.PropertySources
    + org.springframework.core.env.MutablePropertySources
```

## org.springframework.core.ExceptionDepthComparator

```java
org.springframework.core.ExceptionDepthComparator
```

## org.springframework.core.GenericTypeResolver

```java
org.springframework.core.GenericTypeResolver
```

## org.springframework.core.InfrastructureProxy

```java
org.springframework.core.InfrastructureProxy
```

## org.springframework.core.io.buffer.DataBuffer

```java
org.springframework.core.io.buffer.DataBuffer
    + org.springframework.core.io.buffer.DataBufferWrapper
    + org.springframework.core.io.buffer.DefaultDataBuffer
    + org.springframework.core.io.buffer.PooledDataBuffer
        + org.springframework.core.io.buffer.NettyDataBuffer
```

## org.springframework.core.io.buffer.DataBufferFactory

```java
org.springframework.core.io.buffer.DataBufferFactory
    + org.springframework.core.io.buffer.DefaultDataBufferFactory
    + org.springframework.core.io.buffer.NettyDataBufferFactory
```

## org.springframework.core.io.buffer.DataBufferLimitException

```java
org.springframework.core.io.buffer.DataBufferLimitException
```

## org.springframework.core.io.buffer.DataBufferUtils

```java
org.springframework.core.io.buffer.DataBufferUtils
```

## org.springframework.core.io.buffer.DataBufferUtils.Matcher

```java
org.springframework.core.io.buffer.DataBufferUtils.Matcher
```

## org.springframework.core.io.buffer.LimitedDataBufferList

```java
org.springframework.core.io.buffer.LimitedDataBufferList
```

## org.springframework.core.io.InputStreamSource

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

## org.springframework.core.io.ProtocolResolver

```java
org.springframework.core.io.ProtocolResolver
```

## org.springframework.core.io.ResourceEditor

```java
org.springframework.core.io.ResourceEditor
```

## org.springframework.core.io.ResourceLoader

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

## org.springframework.core.io.support.LocalizedResourceHelper

```java
org.springframework.core.io.support.LocalizedResourceHelper
```

## org.springframework.core.io.support.PropertiesLoaderSupport

```java
org.springframework.core.io.support.PropertiesLoaderSupport
    + org.springframework.beans.factory.config.PropertiesFactoryBean
    + org.springframework.beans.factory.config.PropertyResourceConfigurer
        + org.springframework.beans.factory.config.PlaceholderConfigurerSupport
            + org.springframework.beans.factory.config.PropertyPlaceholderConfigurer
                + org.springframework.beans.factory.config.PreferencesPlaceholderConfigurer
            + org.springframework.context.support.PropertySourcesPlaceholderConfigurer
        + org.springframework.beans.factory.config.PropertyOverrideConfigurer
```

## org.springframework.core.io.support.PropertiesLoaderUtils

```java
org.springframework.core.io.support.PropertiesLoaderUtils
```

## org.springframework.core.io.support.PropertySourceFactory

```java
org.springframework.core.io.support.PropertySourceFactory
    + org.springframework.core.io.support.DefaultPropertySourceFactory
```

## org.springframework.core.io.support.ResourceArrayPropertyEditor

```java
org.springframework.core.io.support.ResourceArrayPropertyEditor
```

## org.springframework.core.io.support.ResourcePatternUtils

```java
org.springframework.core.io.support.ResourcePatternUtils
```

## org.springframework.core.io.support.ResourceRegion

```java
org.springframework.core.io.support.ResourceRegion
```

## org.springframework.core.io.support.SpringFactoriesLoader

```java
org.springframework.core.io.support.SpringFactoriesLoader
```

## org.springframework.core.io.VfsUtils

```java
org.springframework.core.io.VfsUtils
```

## org.springframework.core.KotlinDetector

```java
org.springframework.core.KotlinDetector
```

## org.springframework.core.log.LogAccessor

```java
org.springframework.core.log.LogAccessor
```

## org.springframework.core.log.LogDelegateFactory

```java
org.springframework.core.log.LogDelegateFactory
```

## org.springframework.core.log.LogFormatUtils

```java
org.springframework.core.log.LogFormatUtils
```

## org.springframework.core.log.LogMessage

```java
org.springframework.core.log.LogMessage
```

## org.springframework.core.MethodClassKey

```java
org.springframework.core.MethodClassKey
```

## org.springframework.core.MethodIntrospector

```java
org.springframework.core.MethodIntrospector
```

## org.springframework.core.MethodIntrospector.MetadataLookup

```java
org.springframework.core.MethodIntrospector.MetadataLookup
```

## org.springframework.core.MethodParameter

```java
org.springframework.core.MethodParameter
    + org.springframework.core.annotation.SynthesizingMethodParameter
```

## org.springframework.core.metrics.ApplicationStartup

```java
org.springframework.core.metrics.ApplicationStartup
    + org.springframework.core.metrics.jfr.FlightRecorderApplicationStartup
```

## org.springframework.core.metrics.StartupStep

```java
org.springframework.core.metrics.StartupStep
```

## org.springframework.core.metrics.StartupStep.Tag

```java
org.springframework.core.metrics.StartupStep.Tag
```

## org.springframework.core.metrics.StartupStep.Tags

```java
org.springframework.core.metrics.StartupStep.Tags
```

## org.springframework.core.NamedInheritableThreadLocal

```java
org.springframework.core.NamedInheritableThreadLocal
```

## org.springframework.core.NamedThreadLocal

```java
org.springframework.core.NamedThreadLocal
```

## org.springframework.core.NativeDetector

```java
org.springframework.core.NativeDetector
```

## org.springframework.core.NestedCheckedException

```java
org.springframework.core.NestedCheckedException
    + org.springframework.jdbc.support.MetaDataAccessException
```

## org.springframework.core.NestedExceptionUtils

```java
org.springframework.core.NestedExceptionUtils
```

## org.springframework.core.NestedIOException

```java
org.springframework.core.NestedIOException
```

## org.springframework.core.NestedRuntimeException

```java
org.springframework.core.NestedRuntimeException
    + org.springframework.core.annotation.AnnotationConfigurationException
    + org.springframework.aop.framework.AopConfigException
        + org.springframework.aop.aspectj.annotation.NotAnAtAspectException
    + org.springframework.aop.AopInvocationException
    + org.springframework.beans.BeansException
        + org.springframework.beans.factory.BeanNotOfRequiredTypeException
            + org.springframework.beans.factory.BeanIsNotAFactoryException
        + org.springframework.beans.FatalBeanException
            + org.springframework.context.ApplicationContextException
            + org.springframework.beans.factory.BeanCreationException
                + org.springframework.beans.factory.BeanCreationNotAllowedException
                + org.springframework.beans.factory.BeanCurrentlyInCreationException
                + org.springframework.beans.factory.BeanIsAbstractException
                + org.springframework.beans.factory.support.ScopeNotActiveException
                + org.springframework.beans.factory.UnsatisfiedDependencyException
            + org.springframework.beans.factory.BeanDefinitionStoreException
                + org.springframework.beans.factory.support.BeanDefinitionOverrideException
                + org.springframework.beans.factory.parsing.BeanDefinitionParsingException
                + org.springframework.beans.factory.xml.XmlBeanDefinitionStoreException
            + org.springframework.beans.factory.support.BeanDefinitionValidationException
            + org.springframework.beans.factory.BeanExpressionException
            + org.springframework.beans.factory.BeanInitializationException
            + org.springframework.beans.BeanInstantiationException
            + org.springframework.beans.factory.CannotLoadBeanClassException
            + org.springframework.beans.factory.FactoryBeanNotInitializedException
            + org.springframework.beans.InvalidPropertyException
                + org.springframework.beans.NotReadablePropertyException
                + org.springframework.beans.NotWritablePropertyException
                + org.springframework.beans.NullValueInNestedPathException
        + org.springframework.beans.factory.NoSuchBeanDefinitionException
            + org.springframework.beans.factory.NoUniqueBeanDefinitionException
        + org.springframework.beans.PropertyAccessException
            + org.springframework.beans.MethodInvocationException
            + org.springframework.beans.TypeMismatchException
                + org.springframework.beans.ConversionNotSupportedException
                    + org.springframework.web.method.annotation.MethodArgumentConversionNotSupportedException
                + org.springframework.web.method.annotation.MethodArgumentTypeMismatchException
        + org.springframework.beans.PropertyBatchUpdateException
    + org.springframework.scripting.bsh.BshScriptUtils.BshExecutionException
    + org.springframework.core.codec.CodecException
        + org.springframework.core.codec.DecodingException
        + org.springframework.core.codec.EncodingException
    + org.springframework.core.convert.ConversionException
        + org.springframework.core.convert.ConversionFailedException
        + org.springframework.core.convert.ConverterNotFoundException
    + org.springframework.dao.DataAccessException
        + org.springframework.dao.NonTransientDataAccessException
            + org.springframework.dao.CleanupFailureDataAccessException
            + org.springframework.r2dbc.connection.lookup.ConnectionFactoryLookupFailureException
            + org.springframework.dao.DataIntegrityViolationException
                + org.springframework.dao.DuplicateKeyException
            + org.springframework.dao.DataRetrievalFailureException
                + org.springframework.jdbc.IncorrectResultSetColumnCountException
                + org.springframework.dao.IncorrectResultSizeDataAccessException
                    + org.springframework.dao.EmptyResultDataAccessException
                + org.springframework.jdbc.LobRetrievalFailureException
                + org.springframework.orm.ObjectRetrievalFailureException
                    + org.springframework.orm.hibernate5.HibernateObjectRetrievalFailureException
                    + org.springframework.orm.jpa.JpaObjectRetrievalFailureException
            + org.springframework.jdbc.datasource.lookup.DataSourceLookupFailureException
            + org.springframework.dao.InvalidDataAccessApiUsageException
                + org.springframework.jdbc.support.xml.SqlXmlFeatureNotImplementedException
            + org.springframework.dao.InvalidDataAccessResourceUsageException
                + org.springframework.jdbc.BadSqlGrammarException
                + org.springframework.r2dbc.BadSqlGrammarException
                + org.springframework.jca.cci.CciOperationNotSupportedException
                + org.springframework.orm.hibernate5.HibernateQueryException
                + org.springframework.dao.IncorrectUpdateSemanticsDataAccessException
                    + org.springframework.jdbc.JdbcUpdateAffectedIncorrectNumberOfRowsException
                + org.springframework.jca.cci.InvalidResultSetAccessException
                + org.springframework.jdbc.InvalidResultSetAccessException
                + org.springframework.jca.cci.RecordTypeNotSupportedException
                + org.springframework.dao.TypeMismatchDataAccessException
            + org.springframework.r2dbc.core.binding.BindMarkersFactoryResolver.NoBindMarkersFactoryException
            + org.springframework.dao.NonTransientDataAccessResourceException
                + org.springframework.dao.DataAccessResourceFailureException
                    + org.springframework.jca.cci.CannotCreateRecordException
                    + org.springframework.jca.cci.CannotGetCciConnectionException
                    + org.springframework.jdbc.CannotGetJdbcConnectionException
            + org.springframework.dao.PermissionDeniedDataAccessException
            + org.springframework.dao.UncategorizedDataAccessException
                + org.springframework.orm.hibernate5.HibernateJdbcException
                + org.springframework.orm.hibernate5.HibernateSystemException
                + org.springframework.orm.jpa.JpaSystemException
                + org.springframework.jdbc.SQLWarningException
                + org.springframework.r2dbc.UncategorizedR2dbcException
                + org.springframework.jdbc.UncategorizedSQLException
        + org.springframework.dao.RecoverableDataAccessException
        + org.springframework.jdbc.datasource.init.ScriptException
            + org.springframework.jdbc.datasource.init.CannotReadScriptException
            + org.springframework.jdbc.datasource.init.ScriptParseException
            + org.springframework.jdbc.datasource.init.ScriptStatementFailedException
            + org.springframework.jdbc.datasource.init.UncategorizedScriptException
        + org.springframework.r2dbc.connection.init.ScriptException
            + org.springframework.r2dbc.connection.init.CannotReadScriptException
            + org.springframework.r2dbc.connection.init.ScriptParseException
            + org.springframework.r2dbc.connection.init.ScriptStatementFailedException
            + org.springframework.r2dbc.connection.init.UncategorizedScriptException
        + org.springframework.dao.TransientDataAccessException
            + org.springframework.dao.ConcurrencyFailureException
                + org.springframework.dao.OptimisticLockingFailureException
                    + org.springframework.orm.ObjectOptimisticLockingFailureException
                        + org.springframework.orm.hibernate5.HibernateOptimisticLockingFailureException
                        + org.springframework.orm.jpa.JpaOptimisticLockingFailureException
                + org.springframework.dao.PessimisticLockingFailureException
                    + org.springframework.dao.CannotAcquireLockException
                    + org.springframework.dao.CannotSerializeTransactionException
                    + org.springframework.dao.DeadlockLoserDataAccessException
            + org.springframework.dao.QueryTimeoutException
            + org.springframework.dao.TransientDataAccessResourceException
    + org.springframework.ejb.access.EjbAccessException
    + org.springframework.web.socket.server.HandshakeFailureException
    + org.springframework.http.converter.HttpMessageConversionException
        + org.springframework.http.converter.HttpMessageNotReadableException
        + org.springframework.http.converter.HttpMessageNotWritableException
    + org.springframework.jms.JmsException
        + org.springframework.jms.support.destination.DestinationResolutionException
        + org.springframework.jms.IllegalStateException
        + org.springframework.jms.InvalidClientIDException
        + org.springframework.jms.InvalidDestinationException
        + org.springframework.jms.InvalidSelectorException
        + org.springframework.jms.JmsSecurityException
        + org.springframework.jms.listener.adapter.ListenerExecutionFailedException
        + org.springframework.jms.support.converter.MessageConversionException
        + org.springframework.jms.MessageEOFException
        + org.springframework.jms.MessageFormatException
        + org.springframework.jms.MessageNotReadableException
        + org.springframework.jms.MessageNotWriteableException
        + org.springframework.jms.listener.adapter.ReplyFailureException
        + org.springframework.jms.ResourceAllocationException
        + org.springframework.jms.connection.SynchedLocalTransactionFailedException
        + org.springframework.jms.TransactionInProgressException
        + org.springframework.jms.TransactionRolledBackException
        + org.springframework.jms.UncategorizedJmsException
    + org.springframework.jmx.JmxException
        + org.springframework.jmx.export.metadata.InvalidMetadataException
        + org.springframework.jmx.access.InvocationFailureException
        + org.springframework.jmx.access.MBeanConnectFailureException
        + org.springframework.jmx.export.MBeanExportException
            + org.springframework.jmx.export.UnableToRegisterMBeanException
        + org.springframework.jmx.access.MBeanInfoRetrievalException
        + org.springframework.jmx.MBeanServerNotFoundException
        + org.springframework.jmx.export.notification.UnableToSendNotificationException
    + org.springframework.jndi.JndiLookupFailureException
    + org.springframework.scheduling.quartz.JobMethodInvocationFailedException
    + org.springframework.mail.MailException
        + org.springframework.mail.MailAuthenticationException
        + org.springframework.mail.MailParseException
        + org.springframework.mail.MailPreparationException
        + org.springframework.mail.MailSendException
    + org.springframework.messaging.MessagingException
        + org.springframework.messaging.core.DestinationResolutionException
        + org.springframework.messaging.converter.MessageConversionException
        + org.springframework.messaging.MessageDeliveryException
        + org.springframework.messaging.MessageHandlingException
        + org.springframework.messaging.handler.invocation.MethodArgumentResolutionException
            + org.springframework.messaging.handler.annotation.support.MethodArgumentNotValidException
            + org.springframework.messaging.handler.annotation.support.MethodArgumentTypeMismatchException
        + org.springframework.messaging.simp.annotation.support.MissingSessionUserException
    + org.springframework.web.multipart.MultipartException
        + org.springframework.web.multipart.MaxUploadSizeExceededException
    + org.springframework.remoting.RemoteAccessException
        + org.springframework.remoting.RemoteConnectFailureException
        + org.springframework.remoting.RemoteInvocationFailureException
            + org.springframework.remoting.soap.SoapFaultException
                + org.springframework.remoting.jaxws.JaxWsSoapFaultException
        + org.springframework.remoting.RemoteLookupFailureException
        + org.springframework.remoting.RemoteProxyFailureException
        + org.springframework.remoting.RemoteTimeoutException
    + org.springframework.web.server.ResponseStatusException
        + org.springframework.web.server.MediaTypeNotSupportedStatusException
        + org.springframework.web.server.MethodNotAllowedException
        + org.springframework.web.server.NotAcceptableStatusException
        + org.springframework.web.server.ServerErrorException
        + org.springframework.web.server.ServerWebInputException
            + org.springframework.web.bind.support.WebExchangeBindException
        + org.springframework.web.server.UnsupportedMediaTypeStatusException
    + org.springframework.web.client.RestClientException
        + org.springframework.web.client.ResourceAccessException
        + org.springframework.web.client.RestClientResponseException
            + org.springframework.web.client.HttpStatusCodeException
                + org.springframework.web.client.HttpClientErrorException
                    + org.springframework.web.client.HttpClientErrorException.BadRequest
                    + org.springframework.web.client.HttpClientErrorException.Conflict
                    + org.springframework.web.client.HttpClientErrorException.Forbidden
                    + org.springframework.web.client.HttpClientErrorException.Gone
                    + org.springframework.web.client.HttpClientErrorException.MethodNotAllowed
                    + org.springframework.web.client.HttpClientErrorException.NotAcceptable
                    + org.springframework.web.client.HttpClientErrorException.NotFound
                    + org.springframework.web.client.HttpClientErrorException.TooManyRequests
                    + org.springframework.web.client.HttpClientErrorException.Unauthorized
                    + org.springframework.web.client.HttpClientErrorException.UnprocessableEntity
                    + org.springframework.web.client.HttpClientErrorException.UnsupportedMediaType
                + org.springframework.web.client.HttpServerErrorException
                    + org.springframework.web.client.HttpServerErrorException.BadGateway
                    + org.springframework.web.client.HttpServerErrorException.GatewayTimeout
                    + org.springframework.web.client.HttpServerErrorException.InternalServerError
                    + org.springframework.web.client.HttpServerErrorException.NotImplemented
                    + org.springframework.web.client.HttpServerErrorException.ServiceUnavailable
            + org.springframework.web.client.UnknownHttpStatusCodeException
        + org.springframework.web.client.UnknownContentTypeException
    + org.springframework.scheduling.SchedulingException
    + org.springframework.scripting.ScriptCompilationException
    + org.springframework.core.serializer.support.SerializationFailedException
    + org.springframework.web.socket.sockjs.SockJsException
        + org.springframework.web.socket.sockjs.SockJsMessageDeliveryException
        + org.springframework.web.socket.sockjs.SockJsTransportFailureException
    + org.springframework.messaging.simp.stomp.StompConversionException
    + org.springframework.transaction.TransactionException
        + org.springframework.transaction.CannotCreateTransactionException
            + org.springframework.transaction.NestedTransactionNotSupportedException
            + org.springframework.transaction.TransactionSuspensionNotSupportedException
        + org.springframework.transaction.HeuristicCompletionException
        + org.springframework.transaction.TransactionSystemException
        + org.springframework.transaction.TransactionTimedOutException
        + org.springframework.transaction.TransactionUsageException
            + org.springframework.transaction.IllegalTransactionStateException
            + org.springframework.transaction.InvalidIsolationLevelException
            + org.springframework.transaction.InvalidTimeoutException
            + org.springframework.transaction.NoTransactionException
        + org.springframework.transaction.UnexpectedRollbackException
    + org.springframework.web.reactive.function.UnsupportedMediaTypeException
    + org.springframework.web.reactive.function.client.WebClientException
        + org.springframework.web.reactive.function.client.WebClientRequestException
        + org.springframework.web.reactive.function.client.WebClientResponseException
            + org.springframework.web.reactive.function.client.WebClientResponseException.BadGateway
            + org.springframework.web.reactive.function.client.WebClientResponseException.BadRequest
            + org.springframework.web.reactive.function.client.WebClientResponseException.Conflict
            + org.springframework.web.reactive.function.client.WebClientResponseException.Forbidden
            + org.springframework.web.reactive.function.client.WebClientResponseException.GatewayTimeout
            + org.springframework.web.reactive.function.client.WebClientResponseException.Gone
            + org.springframework.web.reactive.function.client.WebClientResponseException.InternalServerError
            + org.springframework.web.reactive.function.client.WebClientResponseException.MethodNotAllowed
            + org.springframework.web.reactive.function.client.WebClientResponseException.NotAcceptable
            + org.springframework.web.reactive.function.client.WebClientResponseException.NotFound
            + org.springframework.web.reactive.function.client.WebClientResponseException.NotImplemented
            + org.springframework.web.reactive.function.client.WebClientResponseException.ServiceUnavailable
            + org.springframework.web.reactive.function.client.WebClientResponseException.TooManyRequests
            + org.springframework.web.reactive.function.client.WebClientResponseException.Unauthorized
            + org.springframework.web.reactive.function.client.UnknownHttpStatusCodeException
            + org.springframework.web.reactive.function.client.WebClientResponseException.UnprocessableEntity
            + org.springframework.web.reactive.function.client.WebClientResponseException.UnsupportedMediaType
    + org.springframework.oxm.XmlMappingException
        + org.springframework.oxm.MarshallingException
            + org.springframework.oxm.MarshallingFailureException
            + org.springframework.oxm.UnmarshallingFailureException
        + org.springframework.oxm.UncategorizedMappingException
        + org.springframework.oxm.ValidationFailureException
```

## org.springframework.core.OrderComparator

```java
org.springframework.core.OrderComparator
    + org.springframework.core.annotation.AnnotationAwareOrderComparator
```

## org.springframework.core.OrderComparator.OrderSourceProvider

```java
org.springframework.core.OrderComparator.OrderSourceProvider
```

## org.springframework.core.Ordered

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

## org.springframework.core.ParameterizedTypeReference

```java
org.springframework.core.ParameterizedTypeReference
```

## org.springframework.core.ParameterNameDiscoverer

```java
org.springframework.core.ParameterNameDiscoverer
    + org.springframework.aop.aspectj.AspectJAdviceParameterNameDiscoverer
    + org.springframework.core.KotlinReflectionParameterNameDiscoverer
    + org.springframework.core.LocalVariableTableParameterNameDiscoverer
    + org.springframework.core.PrioritizedParameterNameDiscoverer
        + org.springframework.core.DefaultParameterNameDiscoverer
    + org.springframework.core.StandardReflectionParameterNameDiscoverer
```

## org.springframework.core.ReactiveAdapter

```java
org.springframework.core.ReactiveAdapter
```

## org.springframework.core.ReactiveAdapterRegistry

```java
org.springframework.core.ReactiveAdapterRegistry
```

## org.springframework.core.ReactiveAdapterRegistry.SpringCoreBlockHoundIntegration

```java
org.springframework.core.ReactiveAdapterRegistry.SpringCoreBlockHoundIntegration
```

## org.springframework.core.ReactiveTypeDescriptor

```java
org.springframework.core.ReactiveTypeDescriptor
```

## org.springframework.core.ResolvableType

```java
org.springframework.core.ResolvableType
```

## org.springframework.core.ResolvableTypeProvider

```java
org.springframework.core.ResolvableTypeProvider
    + org.springframework.context.PayloadApplicationEvent
```

## org.springframework.core.serializer.Deserializer

```java
org.springframework.core.serializer.Deserializer
    + org.springframework.core.serializer.DefaultDeserializer
    + org.springframework.core.serializer.support.SerializationDelegate
```

## org.springframework.core.serializer.Serializer

```java
org.springframework.core.serializer.Serializer
    + org.springframework.core.serializer.DefaultSerializer
    + org.springframework.core.serializer.support.SerializationDelegate
```

## org.springframework.core.SmartClassLoader

```java
org.springframework.core.SmartClassLoader
```

## org.springframework.core.SpringProperties

```java
org.springframework.core.SpringProperties
```

## org.springframework.core.SpringVersion

```java
org.springframework.core.SpringVersion
```

## org.springframework.core.style.StylerUtils

```java
org.springframework.core.style.StylerUtils
```

## org.springframework.core.style.ToStringCreator

```java
org.springframework.core.style.ToStringCreator
```

## org.springframework.core.style.ToStringStyler

```java
org.springframework.core.style.ToStringStyler
    + org.springframework.core.style.DefaultToStringStyler
```

## org.springframework.core.style.ValueStyler

```java
org.springframework.core.style.ValueStyler
    + org.springframework.core.style.DefaultValueStyler
```

## org.springframework.core.task.support.ConcurrentExecutorAdapter

```java
org.springframework.core.task.support.ConcurrentExecutorAdapter
```

## org.springframework.core.task.support.ExecutorServiceAdapter

```java
org.springframework.core.task.support.ExecutorServiceAdapter
```

## org.springframework.core.task.TaskDecorator

```java
org.springframework.core.task.TaskDecorator
```

## org.springframework.core.task.TaskExecutor

```java
org.springframework.core.task.TaskExecutor
    + org.springframework.core.task.AsyncTaskExecutor
        + org.springframework.core.task.AsyncListenableTaskExecutor
            + org.springframework.scheduling.concurrent.ConcurrentTaskExecutor
                + org.springframework.scheduling.concurrent.ConcurrentTaskScheduler
                    + org.springframework.scheduling.concurrent.DefaultManagedTaskScheduler
                + org.springframework.scheduling.concurrent.DefaultManagedTaskExecutor
            + org.springframework.core.task.SimpleAsyncTaskExecutor
            + org.springframework.scheduling.quartz.SimpleThreadPoolTaskExecutor
            + org.springframework.core.task.support.TaskExecutorAdapter
            + org.springframework.scheduling.concurrent.ThreadPoolTaskExecutor
            + org.springframework.scheduling.concurrent.ThreadPoolTaskScheduler
            + org.springframework.jca.work.WorkManagerTaskExecutor
            + org.springframework.scheduling.commonj.WorkManagerTaskExecutor
        + org.springframework.scheduling.SchedulingTaskExecutor
            + org.springframework.scheduling.concurrent.ConcurrentTaskExecutor
                + org.springframework.scheduling.concurrent.ConcurrentTaskScheduler
                    + org.springframework.scheduling.concurrent.DefaultManagedTaskScheduler
                + org.springframework.scheduling.concurrent.DefaultManagedTaskExecutor
            + org.springframework.scheduling.quartz.SimpleThreadPoolTaskExecutor
            + org.springframework.scheduling.concurrent.ThreadPoolTaskExecutor
            + org.springframework.scheduling.concurrent.ThreadPoolTaskScheduler
            + org.springframework.jca.work.WorkManagerTaskExecutor
            + org.springframework.scheduling.commonj.WorkManagerTaskExecutor
    + org.springframework.core.task.SyncTaskExecutor
```

## org.springframework.core.task.TaskRejectedException

```java
org.springframework.core.task.TaskRejectedException
    + org.springframework.core.task.TaskTimeoutException
```

## org.springframework.core.type.AnnotatedTypeMetadata

```java
org.springframework.core.type.AnnotatedTypeMetadata
    + org.springframework.core.type.AnnotationMetadata
        + org.springframework.core.type.classreading.AnnotationMetadataReadingVisitor
        + org.springframework.core.type.StandardAnnotationMetadata
    + org.springframework.core.type.MethodMetadata
        + org.springframework.core.type.classreading.MethodMetadataReadingVisitor
        + org.springframework.core.type.StandardMethodMetadata
```

## org.springframework.core.type.ClassMetadata

```java
org.springframework.core.type.ClassMetadata
    + org.springframework.core.type.AnnotationMetadata
        + org.springframework.core.type.classreading.AnnotationMetadataReadingVisitor
        + org.springframework.core.type.StandardAnnotationMetadata
    + org.springframework.core.type.StandardClassMetadata
        + org.springframework.core.type.StandardAnnotationMetadata
```

## org.springframework.core.type.classreading.MetadataReader

```java
org.springframework.core.type.classreading.MetadataReader
```

## org.springframework.core.type.classreading.MetadataReaderFactory

```java
org.springframework.core.type.classreading.MetadataReaderFactory
    + org.springframework.core.type.classreading.SimpleMetadataReaderFactory
        + org.springframework.core.type.classreading.CachingMetadataReaderFactory
```

## org.springframework.core.type.filter.TypeFilter

```java
org.springframework.core.type.filter.TypeFilter
    + org.springframework.core.type.filter.AbstractClassTestingTypeFilter
        + org.springframework.core.type.filter.RegexPatternTypeFilter
    + org.springframework.core.type.filter.AbstractTypeHierarchyTraversingFilter
        + org.springframework.core.type.filter.AnnotationTypeFilter
        + org.springframework.core.type.filter.AssignableTypeFilter
    + org.springframework.core.type.filter.AspectJTypeFilter
```
