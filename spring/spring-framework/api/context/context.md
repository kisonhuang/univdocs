# context

```java
org.springframework.context.ApplicationContext
org.springframework.context.ApplicationContextAware
org.springframework.context.ApplicationContextException
org.springframework.context.ApplicationContextInitializer
org.springframework.context.ApplicationEvent
org.springframework.context.ApplicationEventPublisher
org.springframework.context.ApplicationEventPublisherAware
org.springframework.context.ApplicationListener
org.springframework.context.ApplicationStartupAware
org.springframework.context.ConfigurableApplicationContext
org.springframework.context.EmbeddedValueResolverAware
org.springframework.context.EnvironmentAware
org.springframework.context.HierarchicalMessageSource
org.springframework.context.Lifecycle
org.springframework.context.LifecycleProcessor
org.springframework.context.MessageSource
org.springframework.context.MessageSourceAware
org.springframework.context.MessageSourceResolvable
org.springframework.context.NoSuchMessageException
org.springframework.context.PayloadApplicationEvent
org.springframework.context.Phased
org.springframework.context.ResourceLoaderAware
org.springframework.context.SmartLifecycle

org.springframework.context.annotation.AdviceMode
org.springframework.context.annotation.AdviceModeImportSelector
org.springframework.context.annotation.AnnotatedBeanDefinitionReader
org.springframework.context.annotation.AnnotationBeanNameGenerator
org.springframework.context.annotation.AnnotationConfigApplicationContext
org.springframework.context.annotation.AnnotationConfigBeanDefinitionParser
org.springframework.context.annotation.AnnotationConfigRegistry
org.springframework.context.annotation.AnnotationConfigUtils
org.springframework.context.annotation.AnnotationScopeMetadataResolver
org.springframework.context.annotation.AutoProxyRegistrar
org.springframework.context.annotation.Bean
org.springframework.context.annotation.ClassPathBeanDefinitionScanner
org.springframework.context.annotation.ClassPathScanningCandidateComponentProvider
org.springframework.context.annotation.CommonAnnotationBeanPostProcessor
org.springframework.context.annotation.CommonAnnotationBeanPostProcessor.LookupElement
org.springframework.context.annotation.ComponentScan
org.springframework.context.annotation.ComponentScan.Filter
org.springframework.context.annotation.ComponentScanBeanDefinitionParser
org.springframework.context.annotation.ComponentScans
org.springframework.context.annotation.Condition
org.springframework.context.annotation.Conditional
org.springframework.context.annotation.ConditionContext
org.springframework.context.annotation.Configuration
org.springframework.context.annotation.ConfigurationClassPostProcessor
org.springframework.context.annotation.ConfigurationCondition
org.springframework.context.annotation.ConfigurationCondition.ConfigurationPhase
org.springframework.context.annotation.ContextAnnotationAutowireCandidateResolver
org.springframework.context.annotation.DeferredImportSelector
org.springframework.context.annotation.DeferredImportSelector.Group
org.springframework.context.annotation.DeferredImportSelector.Group.Entry
org.springframework.context.annotation.DependsOn
org.springframework.context.annotation.Description
org.springframework.context.annotation.EnableAspectJAutoProxy
org.springframework.context.annotation.EnableLoadTimeWeaving
org.springframework.context.annotation.EnableLoadTimeWeaving.AspectJWeaving
org.springframework.context.annotation.EnableMBeanExport
org.springframework.context.annotation.FilterType
org.springframework.context.annotation.FullyQualifiedAnnotationBeanNameGenerator
org.springframework.context.annotation.Import
org.springframework.context.annotation.ImportAware
org.springframework.context.annotation.ImportBeanDefinitionRegistrar
org.springframework.context.annotation.ImportResource
org.springframework.context.annotation.ImportSelector
org.springframework.context.annotation.Jsr330ScopeMetadataResolver
org.springframework.context.annotation.Lazy
org.springframework.context.annotation.LoadTimeWeavingConfiguration
org.springframework.context.annotation.LoadTimeWeavingConfigurer
org.springframework.context.annotation.MBeanExportConfiguration
org.springframework.context.annotation.MBeanExportConfiguration.SpecificPlatform
org.springframework.context.annotation.Primary
org.springframework.context.annotation.Profile
org.springframework.context.annotation.PropertySource
org.springframework.context.annotation.PropertySources
org.springframework.context.annotation.Role
org.springframework.context.annotation.ScannedGenericBeanDefinition
org.springframework.context.annotation.Scope
org.springframework.context.annotation.ScopedProxyMode
org.springframework.context.annotation.ScopeMetadata
org.springframework.context.annotation.ScopeMetadataResolver
org.springframework.context.annotation.TypeFilterUtils

org.springframework.context.config.ContextNamespaceHandler

org.springframework.context.event.AbstractApplicationEventMulticaster
org.springframework.context.event.ApplicationContextEvent
org.springframework.context.event.ApplicationEventMulticaster
org.springframework.context.event.ApplicationListenerMethodAdapter
org.springframework.context.event.ContextClosedEvent
org.springframework.context.event.ContextRefreshedEvent
org.springframework.context.event.ContextStartedEvent
org.springframework.context.event.ContextStoppedEvent
org.springframework.context.event.DefaultEventListenerFactory
org.springframework.context.event.EventListener
org.springframework.context.event.EventListenerFactory
org.springframework.context.event.EventListenerMethodProcessor
org.springframework.context.event.EventPublicationInterceptor
org.springframework.context.event.GenericApplicationListener
org.springframework.context.event.GenericApplicationListenerAdapter
org.springframework.context.event.SimpleApplicationEventMulticaster
org.springframework.context.event.SmartApplicationListener
org.springframework.context.event.SourceFilteringListener

org.springframework.context.expression.AnnotatedElementKey
org.springframework.context.expression.BeanExpressionContextAccessor
org.springframework.context.expression.BeanFactoryAccessor
org.springframework.context.expression.BeanFactoryResolver
org.springframework.context.expression.CachedExpressionEvaluator
org.springframework.context.expression.CachedExpressionEvaluator.ExpressionKey
org.springframework.context.expression.EnvironmentAccessor
org.springframework.context.expression.MapAccessor
org.springframework.context.expression.MethodBasedEvaluationContext
org.springframework.context.expression.StandardBeanExpressionResolver

org.springframework.context.i18n.LocaleContext
org.springframework.context.i18n.LocaleContextHolder
org.springframework.context.i18n.SimpleLocaleContext
org.springframework.context.i18n.SimpleTimeZoneAwareLocaleContext
org.springframework.context.i18n.TimeZoneAwareLocaleContext

org.springframework.context.index.CandidateComponentsIndex
org.springframework.context.index.CandidateComponentsIndexLoader
org.springframework.context.index.processor.CandidateComponentsIndexer

org.springframework.context.support.AbstractApplicationContext
org.springframework.context.support.AbstractMessageSource
org.springframework.context.support.AbstractRefreshableApplicationContext
org.springframework.context.support.AbstractRefreshableConfigApplicationContext
org.springframework.context.support.AbstractResourceBasedMessageSource
org.springframework.context.support.AbstractXmlApplicationContext
org.springframework.context.support.ApplicationObjectSupport
org.springframework.context.support.ClassPathXmlApplicationContext
org.springframework.context.support.ConversionServiceFactoryBean
org.springframework.context.support.DefaultLifecycleProcessor
org.springframework.context.support.DefaultMessageSourceResolvable
org.springframework.context.support.DelegatingMessageSource
org.springframework.context.support.EmbeddedValueResolutionSupport
org.springframework.context.support.FileSystemXmlApplicationContext
org.springframework.context.support.GenericApplicationContext
org.springframework.context.support.GenericGroovyApplicationContext
org.springframework.context.support.GenericXmlApplicationContext
org.springframework.context.support.LiveBeansView
org.springframework.context.support.LiveBeansViewMBean
org.springframework.context.support.MessageSourceAccessor
org.springframework.context.support.MessageSourceResourceBundle
org.springframework.context.support.MessageSourceSupport
org.springframework.context.support.PropertySourcesPlaceholderConfigurer
org.springframework.context.support.ReloadableResourceBundleMessageSource
org.springframework.context.support.ResourceBundleMessageSource
org.springframework.context.support.SimpleThreadScope
org.springframework.context.support.StaticApplicationContext
org.springframework.context.support.StaticMessageSource

org.springframework.context.weaving.AspectJWeavingEnabler
org.springframework.context.weaving.DefaultContextLoadTimeWeaver
org.springframework.context.weaving.LoadTimeWeaverAware
org.springframework.context.weaving.LoadTimeWeaverAwareProcessor
```























