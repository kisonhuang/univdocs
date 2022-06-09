# IoC容器

## 体系结构

```java
+ org.springframework.beans.factory.BeanFactory
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
```

## BeanFactory

```java
String FACTORY_BEAN_PREFIX = "&"

Object getBean(String name)
Object getBean(String name, Object... args)

T getBean(String name, Class<T> requiredType)
T getBean(Class<T> requiredType)
T getBean(Class<T> requiredType, Object... args)

Class<?> getType(String name)
Class<?> getType(String name, boolean allowFactoryBeanInit)

String[] getAliases(String name)

ObjectProvider<T> getBeanProvider(Class<T> requiredType)
ObjectProvider<T> getBeanProvider(ResolvableType requiredType)

boolean containsBean(String name)
boolean isSingleton(String name)
boolean isPrototype(String name)
boolean isTypeMatch(String name, ResolvableType typeToMatch)
boolean isTypeMatch(String name, Class<?> typeToMatch)
```

## HierarchicalBeanFactory

```java
BeanFactory getParentBeanFactory()
boolean containsLocalBean(String name)
```

## ListableBeanFactory

```java
int getBeanDefinitionCount()
String[] getBeanDefinitionNames()
boolean containsBeanDefinition(String beanName)

ObjectProvider<T> getBeanProvider(Class<T> requiredType, boolean allowEagerInit)
ObjectProvider<T> getBeanProvider(ResolvableType requiredType, boolean allowEagerInit)

String[] getBeanNamesForType(Class<?> type)
String[] getBeanNamesForType(Class<?> type, boolean includeNonSingletons, boolean allowEagerInit)
String[] getBeanNamesForType(ResolvableType type)
String[] getBeanNamesForType(ResolvableType type, boolean includeNonSingletons, boolean allowEagerInit)
String[] getBeanNamesForAnnotation(Class<? extends Annotation> annotationType)

Map<String, T> getBeansOfType(Class<T> type)
Map<String, T> getBeansOfType(Class<T> type, boolean includeNonSingletons, boolean allowEagerInit)
Map<String, Object> getBeansWithAnnotation(Class<? extends Annotation> annotationType)

A findAnnotationOnBean(String beanName, Class<A> annotationType)
```

## AutowireCapableBeanFactory

```java
int AUTOWIRE_NO = 0
int AUTOWIRE_BY_NAME = 1
int AUTOWIRE_BY_TYPE = 2
int AUTOWIRE_CONSTRUCTOR = 3
int AUTOWIRE_AUTODETECT = 4

String ORIGINAL_INSTANCE_SUFFIX = ".ORIGINAL"

T createBean(Class<T> beanClass)

void destroyBean(Object existingBean)
void autowireBean(Object existingBean)
void autowireBeanProperties(Object existingBean, int autowireMode, boolean dependencyCheck)
void applyBeanPropertyValues(Object existingBean, String beanName)

Object initializeBean(Object existingBean, String beanName)
Object configureBean(Object existingBean, String beanName)
Object createBean(Class<?> beanClass, int autowireMode, boolean dependencyCheck)
Object autowire(Class<?> beanClass, int autowireMode, boolean dependencyCheck)

Object applyBeanPostProcessorsBeforeInitialization(Object existingBean, String beanName)
Object applyBeanPostProcessorsAfterInitialization(Object existingBean, String beanName)

Object resolveBeanByName(String name, DependencyDescriptor descriptor)
Object resolveDependency(DependencyDescriptor descriptor, String requestingBeanName)
Object resolveDependency(DependencyDescriptor descriptor, String requestingBeanName, Set<String> autowiredBeanNames, TypeConverter typeConverter)

NamedBeanHolder<T> resolveNamedBean(Class<T> requiredType)
```

## ConfigurableBeanFactory

```java
String SCOPE_SINGLETON = "singleton"
String SCOPE_PROTOTYPE = "prototype"

ClassLoader getBeanClassLoader()
void setBeanClassLoader(ClassLoader beanClassLoader)

ClassLoader getTempClassLoader()
void setTempClassLoader(ClassLoader tempClassLoader)

BeanExpressionResolver getBeanExpressionResolver()
void setBeanExpressionResolver(BeanExpressionResolver resolver)

ConversionService getConversionService()
void setConversionService(ConversionService conversionService)

TypeConverter getTypeConverter()
void setTypeConverter(TypeConverter typeConverter)

ApplicationStartup getApplicationStartup()
void setApplicationStartup(ApplicationStartup applicationStartup)

boolean isCacheBeanMetadata()
void setCacheBeanMetadata(boolean cacheBeanMetadata)

boolean isCurrentlyInCreation(String beanName)
void setCurrentlyInCreation(String beanName, boolean inCreation)

boolean hasEmbeddedValueResolver()
void addEmbeddedValueResolver(StringValueResolver valueResolver)

int getBeanPostProcessorCount()
void addBeanPostProcessor(BeanPostProcessor beanPostProcessor)

void registerAlias(String beanName, String alias)
void resolveAliases(StringValueResolver valueResolver)

Scope getRegisteredScope(String scopeName)
void registerScope(String scopeName, Scope scope)

void registerDependentBean(String beanName, String dependentBeanName)
void registerCustomEditor(Class<?> requiredType, Class<? extends PropertyEditor> propertyEditorClass)

void copyRegisteredEditorsTo(PropertyEditorRegistry registry)
void copyConfigurationFrom(ConfigurableBeanFactory otherFactory)

boolean isFactoryBean(String name)
void setParentBeanFactory(BeanFactory parentBeanFactory)
void addPropertyEditorRegistrar(PropertyEditorRegistrar registrar)

void destroyBean(String beanName, Object beanInstance)
void destroyScopedBean(String beanName)
void destroySingletons()

String resolveEmbeddedValue(String value)
String[] getRegisteredScopeNames()
String[] getDependentBeans(String beanName)
String[] getDependenciesForBean(String beanName)

AccessControlContext getAccessControlContext()
BeanDefinition getMergedBeanDefinition(String beanName)
```

## ConfigurableListableBeanFactory

```java
void clearMetadataCache()
void freezeConfiguration()
void preInstantiateSingletons()
void ignoreDependencyType(Class<?> type)
void ignoreDependencyInterface(Class<?> ifc)
void registerResolvableDependency(Class<?> dependencyType, Object autowiredValue)

Iterator<String> getBeanNamesIterator()
BeanDefinition getBeanDefinition(String beanName)

boolean isConfigurationFrozen()
boolean isAutowireCandidate(String beanName, DependencyDescriptor descriptor)
```

## StaticListableBeanFactory

## AbstractBeanFactory

## AbstractAutowireCapableBeanFactory

## DefaultListableBeanFactory

## XmlBeanFactory

## AnnotationConfigApplicationContext

## ApplicationContext

## ConfigurableApplicationContext

## AbstractApplicationContext

## AbstractRefreshableApplicationContext

## AbstractRefreshableConfigApplicationContext

## AbstractXmlApplicationContext

## ClassPathXmlApplicationContext

## FileSystemXmlApplicationContext

## GenericApplicationContext

## GenericGroovyApplicationContext

## GenericXmlApplicationContext

## StaticApplicationContext

## ResourceAdapterApplicationContext

## SimpleJndiBeanFactory

## ConfigurableWebApplicationContext

## AbstractRefreshableWebApplicationContext

## AnnotationConfigWebApplicationContext

## GenericWebApplicationContext

## GroovyWebApplicationContext

## StaticWebApplicationContext

## XmlWebApplicationContext

## WebApplicationContext
















