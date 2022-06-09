# Spring Boot应用程序

```java
org.springframework.boot.autoconfigure.SpringBootApplication
org.springframework.boot.SpringBootConfiguration
org.springframework.boot.autoconfigure.EnableAutoConfiguration
org.springframework.boot.autoconfigure.AutoConfigurationPackage
org.springframework.boot.SpringApplication
org.springframework.boot.autoconfigure.ImportAutoConfiguration

org.springframework.boot.autoconfigure.AutoConfigurationPackages
org.springframework.boot.autoconfigure.AutoConfigurationImportSelector
org.springframework.boot.autoconfigure.AutoConfigurationImportSelector.AutoConfigurationEntry
org.springframework.boot.autoconfigure.AutoConfigurationExcludeFilter
org.springframework.boot.context.TypeExcludeFilter
```

## ImportAutoConfiguration注解

@ImportAutoConfiguration注解用于导入自动配置类。与@EnableAutoConfiguration注解使用相同的排序规则，但是会把自动配置类限制在指定集合中，而不是询问spring.factories。

可以使用exclude来排除不想应用的自动配置类。

优先使用@EnableAutoConfiguration注解，而不是@ImportAutoConfiguration注解，@ImportAutoConfiguration注解在测试时很有用。

```java
org.springframework.boot.autoconfigure.ImportAutoConfiguration
+ value()
+ classes()
+ exclude()
```

## SpringBootApplication注解

添加@SpringBootApplication注解的类：
+ 可以声明一个或多个@Bean方法。
+ 会触发自动配置和组件扫描。

添加@SpringBootApplication注解等同于添加注解：
+ @SpringBootConfiguration
+ @EnableAutoConfiguration
+ @ComponentScan

```java
org.springframework.boot.autoconfigure.SpringBootApplication
+ exclude()
+ excludeName()
+ scanBasePackages()
+ scanBasePackageClasses()
+ nameGenerator()
+ proxyBeanMethods()
```

## SpringBootConfiguration注解

@SpringBootConfiguration注解用于给Spring Boot应用程序提供@Configuration配置类。

@SpringBootConfiguration注解可以替代@Configuration注解，这样就可以自动查找配置。

Spring Boot应用程序只需要提供一个@SpringBootConfiguration配置类，可以从@SpringBootApplication注解中继承@SpringBootConfiguration注解。

```java
org.springframework.boot.SpringBootConfiguration
+ proxyBeanMethods()
```

## EnableAutoConfiguration注解

@EnableAutoConfiguration注解用于启用Spring应用上下文的自动配置，推测并配置可能需要的Bean。
Spring Boot会根据classpath和定义的Bean来应用自动配置类。
例如，如果classpath中包含tomcat-embedded.jar，用户可能需要TomcatServletWebServerFactory，除非用户已经定义了ServletWebServerFactory Bean。

使用@SpringBootApplication时，会自动启用应用上下文的自动配置，此时添加@EnableAutoConfiguration注解不会产生额外效果。

如果定义了自己的配置，自动配置将会失效。
可以使用exclude和excludeName或spring.autoconfigure.exclude属性来排除不想应用的配置。
自动配置将会在用户定义的Bean注册之后应用。

使用@EnableAutoConfiguration注解（通常使用@SpringBootApplication注解）的类所属的包，通常被用作default包。
例如，这个包将会被用于扫描@Entity类。
不使用@SpringBootApplication注解时，建议在根包中使用@EnableAutoConfiguration注解，这样才可以查找所有子包和类。

自动配置类为@Configuration Bean，自动配置类通过SpringFactoriesLoader机制来定位。
自动配置Bean为@Conditional Bean，通常使用@ConditionalOnClass和@ConditionalOnMissingBean注解。

```java
org.springframework.boot.autoconfigure.EnableAutoConfiguration
+ exclude()
+ excludeName()
```

## AutoConfigurationPackage注解

添加@AutoConfigurationPackage注解的类将会使用AutoConfigurationPackages类来注册包。

没有指定basePackages或basePackageClasses时，将会注册添加@AutoConfigurationPackage注解的类所属的包。

```java
org.springframework.boot.autoconfigure.AutoConfigurationPackage
+ basePackages()
+ basePackageClasses()
```

## SpringApplication类

SpringApplication类用于在main方法中启动Spring Boot应用程序。

Spring Boot应用程序的启动步骤：
+ 根据classpath，创建ApplicationContext实例。
+ 注册CommandLinePropertySource，把命令行参数转换为Spring属性。
+ 刷新ApplicationContext，加载所有单例Bean。
+ 触发任何CommandLineRunner Bean。

在main方法中启动Spring Boot应用程序：

```java
@Configuration
@EnableAutoConfiguration
public class MyApplication  {
    // 定义Bean ...

    public static void main(String[] args) {
        SpringApplication.run(MyApplication.class, args);
    }
}
```

创建并定制SpringApplication：

```java
public static void main(String[] args) {
    SpringApplication application = new SpringApplication(MyApplication.class);
    // 定制SpringApplication ...
    application.run(args)
}
```

SpringApplication读取Bean的方式：
+ 通过@Configuration配置类，启动Spring Boot应用程序。
+ 通过AnnotatedBeanDefinitionReader，加载全限定类名。
+ 通过XmlBeanDefinitionReader，加载XML资源的位置。
+ 通过GroovyBeanDefinitionReader，加载Groovy脚本。
+ 通过ClassPathBeanDefinitionScanner，扫描包名。

绑定到SpringApplication的配置属性可以动态设置SpringApplication属性，例如：
+ spring.main.sources=csv文件列表
+ spring.main.web-application-type=none
+ spring.main.banner-mode=off

```java
org.springframework.boot.SpringApplication
+ 静态属性
    + BANNER_LOCATION_PROPERTY
    + BANNER_LOCATION_PROPERTY_VALUE
+ 静态方法
    + main(String[])
    + run(Class<?>, String...)
    + run(Class<?>[], String[])
    + exit(ApplicationContext, ExitCodeGenerator...)
+ 构建函数
    + SpringApplication(Class<?>...)
    + SpringApplication(ResourceLoader, Class<?>...)
+ run方法
    + run(String...)
+ add方法
    + addBootstrapRegistryInitializer(BootstrapRegistryInitializer)
    + addInitializers(ApplicationContextInitializer<?>...)
    + addListeners(ApplicationListener<?>...)
    + addPrimarySources(Collection<Class<?>>)
+ get方法
    + getAdditionalProfiles()
    + getAllSources()
    + getApplicationStartup()
    + getClassLoader()
    + getEnvironmentPrefix()
    + getInitializers()
    + getListeners()
    + getMainApplicationClass()
    + getResourceLoader()
    + getSources()
    + getWebApplicationType()
+ set方法
    + setAddCommandLineProperties(boolean)
    + setAddConversionService(boolean)
    + setAdditionalProfiles(String...)
    + setAllowBeanDefinitionOverriding(boolean)
    + setApplicationContextFactory(ApplicationContextFactory)
    + setApplicationStartup(ApplicationStartup)
    + setBanner(Banner)
    + setBannerMode(Mode)
    + setBeanNameGenerator(BeanNameGenerator)
    + setDefaultProperties(Map<String, Object>)
    + setDefaultProperties(Properties)
    + setEnvironment(ConfigurableEnvironment)
    + setEnvironmentPrefix(String)
    + setHeadless(boolean)
    + setInitializers(Collection<? extends ApplicationContextInitializer<?>>)
    + setLazyInitialization(boolean)
    + setListeners(Collection<? extends ApplicationListener<?>>)
    + setLogStartupInfo(boolean)
    + setMainApplicationClass(Class<?>)
    + setRegisterShutdownHook(boolean)
    + setResourceLoader(ResourceLoader)
    + setSources(Set<String>)
    + setWebApplicationType(WebApplicationType)
+ 废弃属性
    + DEFAULT_CONTEXT_CLASS
    + DEFAULT_REACTIVE_WEB_CONTEXT_CLASS
    + DEFAULT_SERVLET_WEB_CONTEXT_CLASS
+ 废弃方法
    + addBootstrapper(Bootstrapper)
    + setApplicationContextClass(Class<? extends ConfigurableApplicationContext>)
```

## AutoConfigurationPackages类

```java
org.springframework.boot.autoconfigure.AutoConfigurationPackages
+ get(BeanFactory)
+ has(BeanFactory)
+ register(BeanDefinitionRegistry, String...)
```

## AutoConfigurationImportSelector类

```java
org.springframework.boot.autoconfigure.AutoConfigurationImportSelector
+ getExclusionFilter()
+ getImportGroup()
+ getOrder()
+ selectImports(AnnotationMetadata)
+ setBeanClassLoader(ClassLoader)
+ setBeanFactory(BeanFactory)
+ setEnvironment(Environment)
+ setResourceLoader(ResourceLoader)
```

## AutoConfigurationImportSelector.AutoConfigurationEntry类

```java
org.springframework.boot.autoconfigure.AutoConfigurationImportSelector.AutoConfigurationEntry
+ getConfigurations()
+ getExclusions()
```

## AutoConfigurationExcludeFilter类

```java
org.springframework.boot.autoconfigure.AutoConfigurationExcludeFilter
+ match(MetadataReader, MetadataReaderFactory)
+ setBeanClassLoader(ClassLoader)
```

## TypeExcludeFilter类

```java
org.springframework.boot.context.TypeExcludeFilter
+ match(MetadataReader, MetadataReaderFactory)
+ setBeanFactory(BeanFactory)
```




