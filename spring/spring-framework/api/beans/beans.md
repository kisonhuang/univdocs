# beans

## BeanInfoFactory

```java
org.springframework.beans.BeanInfoFactory
    + org.springframework.beans.ExtendedBeanInfoFactory
```

org.springframework.beans.PropertyEditorRegistrar
    + org.springframework.beans.support.ResourceEditorRegistrar

org.springframework.beans.PropertyAccessor
    + org.springframework.beans.ConfigurablePropertyAccessor
        + org.springframework.beans.AbstractPropertyAccessor
            + org.springframework.beans.AbstractNestablePropertyAccessor
                + org.springframework.beans.DirectFieldAccessor
                + org.springframework.beans.BeanWrapperImpl
        + org.springframework.beans.BeanWrapper
            + org.springframework.beans.BeanWrapperImpl

org.springframework.beans.PropertyEditorRegistry
    + org.springframework.beans.ConfigurablePropertyAccessor
        + org.springframework.beans.AbstractPropertyAccessor
            + org.springframework.beans.AbstractNestablePropertyAccessor
                + org.springframework.beans.DirectFieldAccessor
                + org.springframework.beans.BeanWrapperImpl
        + org.springframework.beans.BeanWrapper
            + org.springframework.beans.BeanWrapperImpl
    + org.springframework.beans.PropertyEditorRegistrySupport
        + org.springframework.beans.TypeConverterSupport
            + org.springframework.beans.SimpleTypeConverter
            + org.springframework.beans.AbstractPropertyAccessor
                + org.springframework.beans.AbstractNestablePropertyAccessor
                    + org.springframework.beans.DirectFieldAccessor
                    + org.springframework.beans.BeanWrapperImpl
    + org.springframework.validation.DataBinder
        + org.springframework.web.bind.WebDataBinder
            + org.springframework.web.bind.support.WebRequestDataBinder
            + org.springframework.web.bind.support.WebExchangeDataBinder
            + org.springframework.web.bind.ServletRequestDataBinder
                + org.springframework.web.servlet.mvc.method.annotation.ExtendedServletRequestDataBinder
            
org.springframework.beans.TypeConverter
    + org.springframework.beans.ConfigurablePropertyAccessor
        + org.springframework.beans.AbstractPropertyAccessor
            + org.springframework.beans.AbstractNestablePropertyAccessor
                + org.springframework.beans.DirectFieldAccessor
                + org.springframework.beans.BeanWrapperImpl
        + org.springframework.beans.BeanWrapper
            + org.springframework.beans.BeanWrapperImpl
    + org.springframework.beans.TypeConverterSupport
        + org.springframework.beans.SimpleTypeConverter
        + org.springframework.beans.AbstractPropertyAccessor
            + org.springframework.beans.AbstractNestablePropertyAccessor
                + org.springframework.beans.DirectFieldAccessor
                + org.springframework.beans.BeanWrapperImpl
    + org.springframework.validation.DataBinder
        + org.springframework.web.bind.WebDataBinder
            + org.springframework.web.bind.support.WebRequestDataBinder
            + org.springframework.web.bind.support.WebExchangeDataBinder
            + org.springframework.web.bind.ServletRequestDataBinder
                + org.springframework.web.servlet.mvc.method.annotation.ExtendedServletRequestDataBinder

org.springframework.beans.PropertyValues
    + org.springframework.beans.MutablePropertyValues
        + org.springframework.web.bind.ServletRequestParameterPropertyValues

org.springframework.beans.Mergeable
    + org.springframework.beans.factory.support.ManagedSet
    + org.springframework.beans.factory.support.ManagedMap
    + org.springframework.beans.factory.support.ManagedProperties
    + org.springframework.beans.factory.support.ManagedArray
        + org.springframework.beans.factory.support.ManagedList
    + org.springframework.test.web.servlet.request.MockHttpServletRequestBuilder
        + org.springframework.test.web.servlet.request.MockMultipartHttpServletRequestBuilder

org.springframework.beans.BeanMetadataElement
    + org.springframework.beans.factory.parsing.AliasDefinition
    + org.springframework.beans.factory.config.BeanDefinitionHolder
        + org.springframework.beans.factory.parsing.BeanComponentDefinition
    + org.springframework.beans.BeanMetadataAttribute
    + org.springframework.beans.BeanMetadataAttributeAccessor
        + org.springframework.beans.PropertyValue
        + org.springframework.beans.factory.support.AutowireCandidateQualifier
        + org.springframework.beans.factory.support.AbstractBeanDefinition
            + org.springframework.beans.factory.support.ChildBeanDefinition
            + org.springframework.beans.factory.support.GenericBeanDefinition
                + org.springframework.beans.factory.annotation.AnnotatedGenericBeanDefinition
                + org.springframework.context.annotation.ScannedGenericBeanDefinition
            + org.springframework.beans.factory.support.RootBeanDefinition
    + org.springframework.beans.factory.parsing.ImportDefinition
    + org.springframework.beans.factory.support.ManagedList<E>
        + org.springframework.beans.factory.support.ManagedArray
    + org.springframework.beans.factory.support.ManagedMap<K, V>
    + org.springframework.beans.factory.support.ManagedProperties
    + org.springframework.beans.factory.support.ManagedSet<E>
    + org.springframework.beans.factory.support.MethodOverride
        + org.springframework.beans.factory.support.LookupOverride
        + org.springframework.beans.factory.support.ReplaceOverride
    + org.springframework.beans.factory.config.TypedStringValue
    + org.springframework.beans.factory.config.ConstructorArgumentValues.ValueHolder
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
    + org.springframework.beans.factory.config.BeanReference
        + org.springframework.beans.factory.config.RuntimeBeanNameReference
        + org.springframework.beans.factory.config.RuntimeBeanReference
    + org.springframework.beans.factory.parsing.ComponentDefinition
        + org.springframework.beans.factory.parsing.BeanComponentDefinition
        + org.springframework.beans.factory.parsing.AbstractComponentDefinition
            + org.springframework.aop.config.AdvisorComponentDefinition
            + org.springframework.aop.config.PointcutComponentDefinition
            + org.springframework.beans.factory.parsing.CompositeComponentDefinition
                + org.springframework.aop.config.AspectComponentDefinition
    + org.springframework.beans.factory.parsing.DefaultsDefinition
        + org.springframework.beans.factory.xml.DocumentDefaultsDefinition

org.springframework.beans.factory.BeanFactory
    + org.springframework.jndi.support.SimpleJndiBeanFactory
    + org.springframework.beans.factory.config.AutowireCapableBeanFactory
        + org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory
            + org.springframework.beans.factory.support.DefaultListableBeanFactory
                + org.springframework.beans.factory.xml.XmlBeanFactory
        + org.springframework.beans.factory.config.ConfigurableListableBeanFactory
            + org.springframework.beans.factory.support.DefaultListableBeanFactory
                + org.springframework.beans.factory.xml.XmlBeanFactory
    + org.springframework.beans.factory.HierarchicalBeanFactory
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
        + org.springframework.beans.factory.config.ConfigurableBeanFactory
            + org.springframework.beans.factory.support.AbstractBeanFactory
                + org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory
                    + org.springframework.beans.factory.support.DefaultListableBeanFactory
                        + org.springframework.beans.factory.xml.XmlBeanFactory
            + org.springframework.beans.factory.config.ConfigurableListableBeanFactory
                + org.springframework.beans.factory.support.DefaultListableBeanFactory
                    + org.springframework.beans.factory.xml.XmlBeanFactory
    + org.springframework.beans.factory.ListableBeanFactory
        + org.springframework.beans.factory.support.StaticListableBeanFactory
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
        + org.springframework.beans.factory.config.ConfigurableListableBeanFactory
            + org.springframework.beans.factory.support.DefaultListableBeanFactory
                + org.springframework.beans.factory.xml.XmlBeanFactory

org.springframework.beans.factory.config.BeanFactoryPostProcessor
    + org.springframework.context.weaving.AspectJWeavingEnabler
    + org.springframework.beans.factory.annotation.CustomAutowireConfigurer
    + org.springframework.beans.factory.config.CustomEditorConfigurer
    + org.springframework.beans.factory.config.CustomScopeConfigurer
    + org.springframework.beans.factory.config.DeprecatedBeanWarner
    + org.springframework.context.event.EventListenerMethodProcessor
    + org.springframework.beans.factory.config.PropertyResourceConfigurer
        + org.springframework.beans.factory.config.PlaceholderConfigurerSupport
            + org.springframework.beans.factory.config.PropertyPlaceholderConfigurer
                + org.springframework.beans.factory.config.PreferencesPlaceholderConfigurer
            + org.springframework.context.support.PropertySourcesPlaceholderConfigurer
        + org.springframework.beans.factory.config.PropertyOverrideConfigurer
    + org.springframework.beans.factory.support.BeanDefinitionRegistryPostProcessor
        + org.springframework.context.annotation.ConfigurationClassPostProcessor

org.springframework.beans.factory.support.BeanDefinitionReader
    + org.springframework.beans.factory.support.AbstractBeanDefinitionReader
        + org.springframework.beans.factory.groovy.GroovyBeanDefinitionReader
        + org.springframework.beans.factory.support.PropertiesBeanDefinitionReader
        + org.springframework.beans.factory.xml.XmlBeanDefinitionReader

org.springframework.beans.factory.xml.BeanDefinitionDocumentReader
    + org.springframework.beans.factory.xml.DefaultBeanDefinitionDocumentReader

org.springframework.beans.factory.xml.BeanDefinitionParser
    + org.springframework.beans.factory.xml.AbstractBeanDefinitionParser
        + org.springframework.beans.factory.xml.AbstractSingleBeanDefinitionParser
            + org.springframework.beans.factory.xml.AbstractSimpleBeanDefinitionParser
                + org.springframework.web.servlet.config.GroovyMarkupConfigurerBeanDefinitionParser
                + org.springframework.web.servlet.config.ScriptTemplateConfigurerBeanDefinitionParser
            + org.springframework.scheduling.config.ExecutorBeanDefinitionParser
            + org.springframework.web.servlet.config.FreeMarkerConfigurerBeanDefinitionParser
            + org.springframework.transaction.config.JtaTransactionManagerBeanDefinitionParser
            + org.springframework.scheduling.config.ScheduledTasksBeanDefinitionParser
            + org.springframework.scheduling.config.SchedulerBeanDefinitionParser
            + org.springframework.web.servlet.config.TilesConfigurerBeanDefinitionParser
    + org.springframework.context.annotation.AnnotationConfigBeanDefinitionParser
    + org.springframework.scheduling.config.AnnotationDrivenBeanDefinitionParser
    + org.springframework.context.annotation.ComponentScanBeanDefinitionParser
    + org.springframework.web.servlet.config.CorsBeanDefinitionParser
    + org.springframework.web.servlet.config.ViewResolversBeanDefinitionParser

org.springframework.beans.factory.xml.BeanDefinitionDecorator
    + org.springframework.aop.config.AbstractInterceptorDrivenBeanDefinitionDecorator

org.springframework.beans.factory.config.BeanDefinitionCustomizer

org.springframework.beans.factory.parsing.ReaderEventListener
    + org.springframework.beans.factory.parsing.EmptyReaderEventListener

org.springframework.core.NestedRuntimeException
    + org.springframework.beans.BeansException
        + org.springframework.beans.factory.BeanNotOfRequiredTypeException
            + org.springframework.beans.factory.BeanIsNotAFactoryException
        + org.springframework.beans.FatalBeanException
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
        + org.springframework.beans.PropertyBatchUpdateException

org.springframework.beans.factory.FactoryBean<T>
    + org.springframework.beans.factory.config.AbstractFactoryBean<T>
        + org.springframework.beans.factory.serviceloader.AbstractServiceLoaderBasedFactoryBean
            + org.springframework.beans.factory.serviceloader.ServiceFactoryBean
            + org.springframework.beans.factory.serviceloader.ServiceListFactoryBean
            + org.springframework.beans.factory.serviceloader.ServiceLoaderFactoryBean
        + org.springframework.beans.factory.config.ListFactoryBean
        + org.springframework.beans.factory.config.MapFactoryBean
        + org.springframework.beans.factory.config.ObjectFactoryCreatingFactoryBean
        + org.springframework.beans.factory.config.ProviderCreatingFactoryBean
        + org.springframework.beans.factory.config.SetFactoryBean
    + org.springframework.beans.factory.config.FieldRetrievingFactoryBean
    + org.springframework.beans.factory.config.MethodInvokingFactoryBean
    + org.springframework.beans.factory.config.PropertiesFactoryBean
    + org.springframework.beans.factory.config.PropertyPathFactoryBean
    + org.springframework.beans.factory.config.ServiceLocatorFactoryBean
    + org.springframework.beans.factory.config.YamlMapFactoryBean
    + org.springframework.beans.factory.config.YamlPropertiesFactoryBean
    + org.springframework.beans.factory.SmartFactoryBean<T>


org.springframework.beans.factory.config.BeanExpressionResolver
    + org.springframework.context.expression.StandardBeanExpressionResolver


org.springframework.beans.factory.Aware
    + org.springframework.beans.factory.BeanClassLoaderAware
    + org.springframework.beans.factory.BeanFactoryAware
    + org.springframework.beans.factory.BeanNameAware

org.springframework.beans.annotation.AnnotationBeanUtils
org.springframework.beans.BeanUtils
org.springframework.beans.factory.annotation.BeanFactoryAnnotationUtils
org.springframework.beans.factory.BeanFactoryUtils
org.springframework.beans.factory.support.BeanDefinitionReaderUtils
org.springframework.beans.PropertyAccessorUtils














