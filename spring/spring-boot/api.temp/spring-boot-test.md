# Test 150

```java
org.springframework.boot.test.context.runner.AbstractApplicationContextRunner
    + org.springframework.boot.test.context.runner.ApplicationContextRunner
    + org.springframework.boot.test.context.runner.WebApplicationContextRunner
    + org.springframework.boot.test.context.runner.ReactiveWebApplicationContextRunner

+ org.springframework.boot.test.autoconfigure.filter.AnnotationCustomizableTypeExcludeFilter
    + org.springframework.boot.test.autoconfigure.filter.StandardAnnotationCustomizableTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.data.jdbc.DataJdbcTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.data.redis.DataRedisTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.data.mongo.DataMongoTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.data.ldap.DataLdapTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.data.neo4j.DataNeo4jTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.jdbc.JdbcTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.json.JsonTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.jooq.JooqTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.orm.jpa.DataJpaTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.web.client.RestClientTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.web.reactive.WebFluxTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.web.servlet.WebMvcTypeExcludeFilter
        + org.springframework.boot.test.autoconfigure.webservices.client.WebServiceClientExcludeFilter
```



## AnnotationCustomizableTypeExcludeFilterç±»

```java
org.springframework.boot.test.autoconfigure.filter.AnnotationCustomizableTypeExcludeFilter
+ match(MetadataReader, MetadataReaderFactory)
+ setBeanClassLoader(ClassLoader)
```




# Spring Boot API

## æ³¨è§£

org.springframework.boot.test.autoconfigure.OverrideAutoConfiguration
org.springframework.boot.test.autoconfigure.actuate.metrics.AutoConfigureMetrics
org.springframework.boot.test.autoconfigure.core.AutoConfigureCache
org.springframework.boot.test.autoconfigure.data.cassandra.AutoConfigureDataCassandra
org.springframework.boot.test.autoconfigure.data.cassandra.DataCassandraTest
org.springframework.boot.test.autoconfigure.data.jdbc.AutoConfigureDataJdbc
org.springframework.boot.test.autoconfigure.data.jdbc.DataJdbcTest
org.springframework.boot.test.autoconfigure.data.ldap.AutoConfigureDataLdap
org.springframework.boot.test.autoconfigure.data.ldap.DataLdapTest
org.springframework.boot.test.autoconfigure.data.mongo.AutoConfigureDataMongo
org.springframework.boot.test.autoconfigure.data.mongo.DataMongoTest
org.springframework.boot.test.autoconfigure.data.neo4j.AutoConfigureDataNeo4j
org.springframework.boot.test.autoconfigure.data.neo4j.DataNeo4jTest
org.springframework.boot.test.autoconfigure.data.r2dbc.AutoConfigureDataR2dbc
org.springframework.boot.test.autoconfigure.data.r2dbc.DataR2dbcTest
org.springframework.boot.test.autoconfigure.data.redis.AutoConfigureDataRedis
org.springframework.boot.test.autoconfigure.data.redis.DataRedisTest
org.springframework.boot.test.autoconfigure.filter.TypeExcludeFilters
org.springframework.boot.test.autoconfigure.jdbc.AutoConfigureJdbc
org.springframework.boot.test.autoconfigure.jdbc.AutoConfigureTestDatabase
org.springframework.boot.test.autoconfigure.jdbc.JdbcTest
org.springframework.boot.test.autoconfigure.jooq.AutoConfigureJooq
org.springframework.boot.test.autoconfigure.jooq.JooqTest
org.springframework.boot.test.autoconfigure.json.AutoConfigureJson
org.springframework.boot.test.autoconfigure.json.AutoConfigureJsonTesters
org.springframework.boot.test.autoconfigure.json.JsonTest
org.springframework.boot.test.autoconfigure.orm.jpa.AutoConfigureDataJpa
org.springframework.boot.test.autoconfigure.orm.jpa.AutoConfigureTestEntityManager
org.springframework.boot.test.autoconfigure.orm.jpa.DataJpaTest
org.springframework.boot.test.autoconfigure.properties.PropertyMapping
org.springframework.boot.test.autoconfigure.restdocs.AutoConfigureRestDocs
org.springframework.boot.test.autoconfigure.web.client.AutoConfigureMockRestServiceServer
org.springframework.boot.test.autoconfigure.web.client.AutoConfigureWebClient
org.springframework.boot.test.autoconfigure.web.client.RestClientTest
org.springframework.boot.test.autoconfigure.web.reactive.AutoConfigureWebFlux
org.springframework.boot.test.autoconfigure.web.reactive.AutoConfigureWebTestClient
org.springframework.boot.test.autoconfigure.web.reactive.WebFluxTest
org.springframework.boot.test.autoconfigure.web.servlet.AutoConfigureMockMvc
org.springframework.boot.test.autoconfigure.web.servlet.AutoConfigureWebMvc
org.springframework.boot.test.autoconfigure.web.servlet.WebMvcTest
org.springframework.boot.test.autoconfigure.webservices.client.AutoConfigureMockWebServiceServer
org.springframework.boot.test.autoconfigure.webservices.client.AutoConfigureWebServiceClient
org.springframework.boot.test.autoconfigure.webservices.client.WebServiceClientTest
org.springframework.boot.test.context.SpringBootTest
org.springframework.boot.test.context.TestComponent
org.springframework.boot.test.context.TestConfiguration
org.springframework.boot.test.mock.mockito.MockBean
org.springframework.boot.test.mock.mockito.MockBeans
org.springframework.boot.test.mock.mockito.SpyBean
org.springframework.boot.test.mock.mockito.SpyBeans

## æä¸¾

org.springframework.boot.test.autoconfigure.filter.AnnotationCustomizableTypeExcludeFilter.FilterType
org.springframework.boot.test.autoconfigure.jdbc.AutoConfigureTestDatabase.Replace
org.springframework.boot.test.autoconfigure.properties.SkipPropertyMapping
org.springframework.boot.test.autoconfigure.web.servlet.MockMvcPrint
org.springframework.boot.test.context.SpringBootTest.WebEnvironment
org.springframework.boot.test.context.assertj.ApplicationContextAssert.Scope
org.springframework.boot.test.mock.mockito.MockReset
org.springframework.boot.test.util.TestPropertyValues.Type
org.springframework.boot.test.web.client.TestRestTemplate.HttpClientOption

## æ¥å£

org.springframework.boot.test.autoconfigure.restdocs.RestDocsMockMvcConfigurationCustomizer
org.springframework.boot.test.autoconfigure.restdocs.RestDocsRestAssuredConfigurationCustomizer
org.springframework.boot.test.autoconfigure.restdocs.RestDocsWebTestClientConfigurationCustomizer
org.springframework.boot.test.autoconfigure.web.servlet.MockMvcBuilderCustomizer
org.springframework.boot.test.context.DefaultTestExecutionListenersPostProcessor
org.springframework.boot.test.context.assertj.ApplicationContextAssertProvider<C extends ApplicationContext>
org.springframework.boot.test.context.assertj.AssertableApplicationContext
org.springframework.boot.test.context.assertj.AssertableReactiveWebApplicationContext
org.springframework.boot.test.context.assertj.AssertableWebApplicationContext
org.springframework.boot.test.context.runner.ContextConsumer<C extends ApplicationContext>
org.springframework.boot.test.system.CapturedOutput
org.springframework.boot.test.web.reactive.server.WebTestClientBuilderCustomizer

## ç±»

org.springframework.boot.test.autoconfigure.SpringBootDependencyInjectionTestExecutionListener






org.springframework.boot.test.autoconfigure.filter.FilterAnnotations


org.springframework.boot.test.autoconfigure.jdbc.TestDatabaseAutoConfiguration

org.springframework.boot.test.autoconfigure.json.JsonTestersAutoConfiguration


org.springframework.boot.test.autoconfigure.orm.jpa.TestEntityManager
org.springframework.boot.test.autoconfigure.orm.jpa.TestEntityManagerAutoConfiguration
org.springframework.boot.test.autoconfigure.properties.AnnotationsPropertySource
org.springframework.boot.test.autoconfigure.restdocs.RestDocsAutoConfiguration
org.springframework.boot.test.autoconfigure.restdocs.RestDocsMockMvcBuilderCustomizer
org.springframework.boot.test.autoconfigure.restdocs.RestDocsProperties
org.springframework.boot.test.autoconfigure.restdocs.RestDocsTestExecutionListener
org.springframework.boot.test.autoconfigure.web.client.MockRestServiceServerAutoConfiguration

org.springframework.boot.test.autoconfigure.web.client.WebClientRestTemplateAutoConfiguration
org.springframework.boot.test.autoconfigure.web.reactive.SpringBootWebTestClientBuilderCustomizer

org.springframework.boot.test.autoconfigure.web.reactive.WebTestClientAutoConfiguration
org.springframework.boot.test.autoconfigure.web.servlet.MockMvcAutoConfiguration
org.springframework.boot.test.autoconfigure.web.servlet.MockMvcWebClientAutoConfiguration
org.springframework.boot.test.autoconfigure.web.servlet.MockMvcWebDriverAutoConfiguration
org.springframework.boot.test.autoconfigure.web.servlet.SpringBootMockMvcBuilderCustomizer

org.springframework.boot.test.autoconfigure.webservices.client.MockWebServiceServerAutoConfiguration
org.springframework.boot.test.autoconfigure.webservices.client.MockWebServiceServerTestExecutionListener

org.springframework.boot.test.autoconfigure.webservices.client.WebServiceClientTemplateAutoConfiguration
org.springframework.boot.test.context.AnnotatedClassFinder
org.springframework.boot.test.context.ConfigDataApplicationContextInitializer
org.springframework.boot.test.context.ConfigFileApplicationContextInitializer
org.springframework.boot.test.context.FilteredClassLoader
org.springframework.boot.test.context.FilteredClassLoader.ClassFilter
org.springframework.boot.test.context.FilteredClassLoader.ClassPathResourceFilter
org.springframework.boot.test.context.FilteredClassLoader.PackageFilter
org.springframework.boot.test.context.ReactiveWebMergedContextConfiguration
org.springframework.boot.test.context.SpringBootContextLoader
org.springframework.boot.test.context.SpringBootTestContextBootstrapper
org.springframework.boot.test.context.assertj.ApplicationContextAssert<C extends ApplicationContext>
org.springframework.boot.test.json.AbstractJsonMarshalTester.FieldInitializer<M>
org.springframework.boot.test.json.AbstractJsonMarshalTester<T>
org.springframework.boot.test.json.BasicJsonTester
org.springframework.boot.test.json.GsonTester<T>
org.springframework.boot.test.json.JacksonTester<T>
org.springframework.boot.test.json.JsonContent<T>
org.springframework.boot.test.json.JsonContentAssert
org.springframework.boot.test.json.JsonbTester<T>
org.springframework.boot.test.json.ObjectContent<T>
org.springframework.boot.test.json.ObjectContentAssert<A>
org.springframework.boot.test.mock.mockito.MockitoPostProcessor
org.springframework.boot.test.mock.mockito.MockitoTestExecutionListener
org.springframework.boot.test.mock.mockito.ResetMocksTestExecutionListener
org.springframework.boot.test.mock.mockito.SpringBootMockResolver
org.springframework.boot.test.mock.web.SpringBootMockServletContext
org.springframework.boot.test.system.OutputCaptureExtension
org.springframework.boot.test.system.OutputCaptureRule
org.springframework.boot.test.util.ApplicationContextTestUtils
org.springframework.boot.test.util.TestPropertyValues
org.springframework.boot.test.util.TestPropertyValues.Pair
org.springframework.boot.test.web.client.LocalHostUriTemplateHandler
org.springframework.boot.test.web.client.MockServerRestTemplateCustomizer
org.springframework.boot.test.web.client.RootUriRequestExpectationManager
org.springframework.boot.test.web.client.TestRestTemplate
org.springframework.boot.test.web.client.TestRestTemplate.CustomHttpComponentsClientHttpRequestFactory
org.springframework.boot.test.web.htmlunit.LocalHostWebClient
org.springframework.boot.test.web.htmlunit.webdriver.LocalHostWebConnectionHtmlUnitDriver


















