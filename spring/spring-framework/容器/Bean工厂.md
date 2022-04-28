# Bean工厂

```java
org.springframework.beans.factory.BeanFactory

org.springframework.beans.factory.ListableBeanFactory
org.springframework.beans.factory.HierarchicalBeanFactory
org.springframework.beans.factory.config.AutowireCapableBeanFactory

org.springframework.beans.factory.config.ConfigurableBeanFactory
org.springframework.beans.factory.config.ConfigurableListableBeanFactory

org.springframework.beans.factory.support.AbstractBeanFactory
org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory

org.springframework.beans.factory.support.DefaultListableBeanFactory
org.springframework.beans.factory.xml.XmlBeanFactory

org.springframework.beans.factory.support.StaticListableBeanFactory
org.springframework.jndi.support.SimpleJndiBeanFactory
```

## BeanFactory

```java
FACTORY_BEAN_PREFIX = "&"
containsBean(String name)

getBean(String name)
getBean(String name, Class<T> requiredType)
getBean(String name, Object... args)
getBean(Class<T> requiredType)
getBean(Class<T> requiredType, Object... args)

getBeanProvider(Class<T> requiredType)
getBeanProvider(ResolvableType requiredType)

getType(String name)
getType(String name, boolean allowFactoryBeanInit)
getAliases(String name)

isSingleton(String name)
isPrototype(String name)
isTypeMatch(String name, ResolvableType typeToMatch)
isTypeMatch(String name, Class<?> typeToMatch)
```

## ListableBeanFactory

```java
containsBeanDefinition(String beanName)

getBeanDefinitionCount()
getBeanDefinitionNames()

getBeanProvider(Class<T> requiredType, boolean allowEagerInit)
getBeanProvider(ResolvableType requiredType, boolean allowEagerInit)

getBeanNamesForType(ResolvableType type)
getBeanNamesForType(ResolvableType type, boolean includeNonSingletons, boolean allowEagerInit)
getBeanNamesForType(Class<?> type)
getBeanNamesForType(Class<?> type, boolean includeNonSingletons, boolean allowEagerInit)
getBeanNamesForAnnotation(Class<? extends Annotation> annotationType)

getBeansOfType(Class<T> type)
getBeansOfType(Class<T> type, boolean includeNonSingletons, boolean allowEagerInit)
getBeansWithAnnotation(Class<? extends Annotation> annotationType)

findAnnotationOnBean(String beanName, Class<A> annotationType)
findAnnotationOnBean(String beanName, Class<A> annotationType, boolean allowFactoryBeanInit)
```

## HierarchicalBeanFactory

```java
containsLocalBean(String name)
getParentBeanFactory()
```

## AutowireCapableBeanFactory

```java
AUTOWIRE_NO          = 0
AUTOWIRE_BY_NAME     = 1
AUTOWIRE_BY_TYPE     = 2
AUTOWIRE_CONSTRUCTOR = 3
AUTOWIRE_AUTODETECT  = 4

ORIGINAL_INSTANCE_SUFFIX = ".ORIGINAL"

initializeBean(Object existingBean, String beanName)
configureBean(Object existingBean, String beanName)
destroyBean(Object existingBean)

createBean(Class<T> beanClass)
createBean(Class<?> beanClass, int autowireMode, boolean dependencyCheck)

autowire(Class<?> beanClass, int autowireMode, boolean dependencyCheck)
autowireBean(Object existingBean)
autowireBeanProperties(Object existingBean, int autowireMode, boolean dependencyCheck)

applyBeanPropertyValues(Object existingBean, String beanName)
applyBeanPostProcessorsBeforeInitialization(Object existingBean, String beanName)
applyBeanPostProcessorsAfterInitialization(Object existingBean, String beanName)

resolveNamedBean(Class<T> requiredType)
resolveBeanByName(String name, DependencyDescriptor descriptor)
resolveDependency(DependencyDescriptor descriptor, String requestingBeanName)
resolveDependency(DependencyDescriptor descriptor, String requestingBeanName, Set<String> autowiredBeanNames, TypeConverter typeConverter)
```

## ConfigurableBeanFactory

```java
SCOPE_SINGLETON = "singleton"
SCOPE_PROTOTYPE = "prototype"

addPropertyEditorRegistrar(PropertyEditorRegistrar registrar)
addEmbeddedValueResolver(StringValueResolver valueResolver)
addBeanPostProcessor(BeanPostProcessor beanPostProcessor)

copyConfigurationFrom(ConfigurableBeanFactory otherFactory)
copyRegisteredEditorsTo(PropertyEditorRegistry registry)

registerAlias(String beanName, String alias)
registerScope(String scopeName, Scope scope)
registerDependentBean(String beanName, String dependentBeanName)
registerCustomEditor(Class<?> requiredType, Class<? extends PropertyEditor> propertyEditorClass)

resolveAliases(StringValueResolver valueResolver)
resolveEmbeddedValue(String value)

destroyBean(String beanName, Object beanInstance)
destroyScopedBean(String beanName)
destroySingletons()

setApplicationStartup(ApplicationStartup applicationStartup)
setBeanClassLoader(ClassLoader beanClassLoader)
setBeanExpressionResolver(BeanExpressionResolver resolver)
setCacheBeanMetadata(boolean cacheBeanMetadata)
setConversionService(ConversionService conversionService)
setCurrentlyInCreation(String beanName, boolean inCreation)
setParentBeanFactory(BeanFactory parentBeanFactory)
setTempClassLoader(ClassLoader tempClassLoader)
setTypeConverter(TypeConverter typeConverter)

getAccessControlContext()
getApplicationStartup()
getBeanClassLoader()
getBeanExpressionResolver()
getBeanPostProcessorCount()
getConversionService()
getDependenciesForBean(String beanName)
getDependentBeans(String beanName)
getMergedBeanDefinition(String beanName)
getRegisteredScope(String scopeName)
getRegisteredScopeNames()
getTempClassLoader()
getTypeConverter()

hasEmbeddedValueResolver()
isCacheBeanMetadata()
isCurrentlyInCreation(String beanName)
isFactoryBean(String name)
```

## ConfigurableListableBeanFactory

```java

ignoreDependencyType(Class<?> type)
ignoreDependencyInterface(Class<?> ifc)

clearMetadataCache()
freezeConfiguration()
preInstantiateSingletons()
registerResolvableDependency(Class<?> dependencyType, Object autowiredValue)

getBeanDefinition(String beanName)
getBeanNamesIterator()

isConfigurationFrozen()
isAutowireCandidate(String beanName, DependencyDescriptor descriptor)
```






















