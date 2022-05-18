# SpringApplication

## SpringApplication

```java
org.springframework.boot.SpringApplication

org.springframework.boot.Banner
   + org.springframework.boot.ImageBanner
   + org.springframework.boot.ResourceBanner

org.springframework.boot.Banner.Mode
org.springframework.boot.ImageBanner.PixelMode

org.springframework.boot.WebApplicationType

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
org.springframework.boot.ApplicationContextFactory


org.springframework.boot.ApplicationArguments
    + org.springframework.boot.DefaultApplicationArguments

org.springframework.boot.ApplicationRunner
    + org.springframework.boot.autoconfigure.batch.JobLauncherApplicationRunner

org.springframework.boot.CommandLineRunner

org.springframework.boot.DefaultPropertiesPropertySource

org.springframework.boot.ExitCodeEvent
org.springframework.boot.ExitCodeExceptionMapper

org.springframework.boot.ExitCodeGenerator
    + org.springframework.boot.autoconfigure.batch.JobExecutionExitCodeGenerator

org.springframework.boot.LazyInitializationBeanFactoryPostProcessor
org.springframework.boot.LazyInitializationExcludeFilter

org.springframework.boot.SpringApplicationRunListener
    + org.springframework.boot.context.event.EventPublishingRunListener

org.springframework.boot.SpringApplicationShutdownHandlers
org.springframework.boot.SpringBootExceptionReporter
org.springframework.boot.SpringBootVersion











```

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






















