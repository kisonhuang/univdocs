## Bean生命周期

## 初始化方法及其顺序

```java
BeanNameAware.setBeanName(String name)
BeanClassLoaderAware.setBeanClassLoader(ClassLoader classLoader)
BeanFactoryAware.setBeanFactory(BeanFactory beanFactory)
EnvironmentAware.setEnvironment(Environment environment)
EmbeddedValueResolverAware.setEmbeddedValueResolver(StringValueResolver resolver)
ResourceLoaderAware.setResourceLoader(ResourceLoader resourceLoader)                                             (ApplicationContext) 
ApplicationEventPublisherAware.setApplicationEventPublisher(ApplicationEventPublisher applicationEventPublisher) (ApplicationContext) 
MessageSourceAware.setMessageSource(MessageSource messageSource)                                                 (ApplicationContext) 
ApplicationContextAware.setApplicationContext(ApplicationContext applicationContext)                             (ApplicationContext) 
ServletContextAware.setServletContext(ServletContext servletContext)                                             (WebApplicationContext)
BeanPostProcessor.postProcessBeforeInitialization(Object bean, String beanName)
InitializingBean.afterPropertiesSet()
自定义init-method
BeanPostProcessor.postProcessAfterInitialization(Object bean, String beanName)
```

## 销毁方法及其顺序

```java
DestructionAwareBeanPostProcessor.postProcessBeforeDestruction(Object bean, String beanName)
DisposableBean.destroy()
自定义destroy-method
```




