# Web




org.springframework.boot.autoconfigure.web.client.RestTemplateBuilderConfigurer
org.springframework.boot.autoconfigure.web.ConditionalOnEnabledResourceChain
org.springframework.boot.autoconfigure.web.format.DateTimeFormatters
org.springframework.boot.autoconfigure.web.format.WebConversionService


org.springframework.boot.autoconfigure.web.reactive.function.client.ReactorNettyHttpClientMapper
org.springframework.boot.autoconfigure.web.reactive.function.client.WebClientCodecCustomizer
org.springframework.boot.autoconfigure.web.reactive.ResourceHandlerRegistrationCustomizer
org.springframework.boot.autoconfigure.web.reactive.WebFluxRegistrations







org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration.DispatcherServletConfiguration
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration.DispatcherServletRegistrationConfiguration

org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration.WhitelabelErrorViewConfiguration

org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration

org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration

org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration.EnableWebMvcConfiguration
org.springframework.boot.autoconfigure.web.servlet.WebMvcAutoConfiguration.WebMvcAutoConfigurationAdapter

org.springframework.boot.autoconfigure.web.servlet.MultipartProperties
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.Async
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.Contentnegotiation
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.Format
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.MatchingStrategy
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.Pathmatch
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.Servlet
org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties.View

org.springframework.boot.autoconfigure.web.servlet.ConditionalOnMissingFilterBean
org.springframework.boot.autoconfigure.web.servlet.DefaultJerseyApplicationPath
org.springframework.boot.autoconfigure.web.servlet.DispatcherServletPath
org.springframework.boot.autoconfigure.web.servlet.error.DefaultErrorViewResolver
org.springframework.boot.autoconfigure.web.servlet.error.ErrorViewResolver
org.springframework.boot.autoconfigure.web.servlet.JerseyApplicationPath
org.springframework.boot.autoconfigure.web.servlet.JspTemplateAvailabilityProvider
org.springframework.boot.autoconfigure.web.servlet.WebMvcRegistrations


org.springframework.boot.autoconfigure.web.client.RestTemplateAutoConfiguration

org.springframework.boot.autoconfigure.web.reactive.error.ErrorWebFluxAutoConfiguration
org.springframework.boot.autoconfigure.web.reactive.function.client.ClientHttpConnectorAutoConfiguration
org.springframework.boot.autoconfigure.web.reactive.function.client.WebClientAutoConfiguration
org.springframework.boot.autoconfigure.web.reactive.function.client.WebClientAutoConfiguration.WebClientCodecsConfiguration
org.springframework.boot.autoconfigure.web.reactive.HttpHandlerAutoConfiguration
org.springframework.boot.autoconfigure.web.reactive.HttpHandlerAutoConfiguration.AnnotationConfig
org.springframework.boot.autoconfigure.web.reactive.ReactiveMultipartAutoConfiguration
org.springframework.boot.autoconfigure.web.reactive.WebFluxAutoConfiguration
org.springframework.boot.autoconfigure.web.reactive.WebFluxAutoConfiguration.EnableWebFluxConfiguration
org.springframework.boot.autoconfigure.web.reactive.WebFluxAutoConfiguration.WebFluxConfig
org.springframework.boot.autoconfigure.web.reactive.WebFluxAutoConfiguration.WelcomePageConfiguration
org.springframework.boot.autoconfigure.web.reactive.WebSessionIdResolverAutoConfiguration



org.springframework.boot.autoconfigure.web.ErrorProperties
org.springframework.boot.autoconfigure.web.ErrorProperties.IncludeAttribute
org.springframework.boot.autoconfigure.web.ErrorProperties.IncludeStacktrace
org.springframework.boot.autoconfigure.web.ErrorProperties.Whitelabel
org.springframework.boot.autoconfigure.web.reactive.ReactiveMultipartProperties
org.springframework.boot.autoconfigure.web.reactive.WebFluxProperties
org.springframework.boot.autoconfigure.web.reactive.WebFluxProperties.Cookie
org.springframework.boot.autoconfigure.web.reactive.WebFluxProperties.Format
org.springframework.boot.autoconfigure.web.reactive.WebFluxProperties.SameSite
org.springframework.boot.autoconfigure.web.reactive.WebFluxProperties.Session
org.springframework.boot.autoconfigure.web.WebProperties
org.springframework.boot.autoconfigure.web.WebProperties.LocaleResolver
org.springframework.boot.autoconfigure.web.WebProperties.Resources
org.springframework.boot.autoconfigure.web.WebProperties.Resources.Cache
org.springframework.boot.autoconfigure.web.WebProperties.Resources.Cache.Cachecontrol
org.springframework.boot.autoconfigure.web.WebProperties.Resources.Chain
org.springframework.boot.autoconfigure.web.WebProperties.Resources.Chain.Strategy
org.springframework.boot.autoconfigure.web.WebProperties.Resources.Chain.Strategy.Content
org.springframework.boot.autoconfigure.web.WebProperties.Resources.Chain.Strategy.Fixed






=======================================================


org.springframework.boot.web.context.ServerPortInfoApplicationContextInitializer
org.springframework.boot.web.servlet.support.ServletContextApplicationContextInitializer

org.springframework.boot.web.context.WebServerApplicationContext
    + org.springframework.boot.web.context.ConfigurableWebServerApplicationContext
        + org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext
            + org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext
            + org.springframework.boot.web.servlet.context.XmlServletWebServerApplicationContext
        + org.springframework.boot.web.reactive.context.ReactiveWebServerApplicationContext
            + org.springframework.boot.web.reactive.context.AnnotationConfigReactiveWebServerApplicationContext

org.springframework.boot.web.servlet.context.AnnotationConfigServletWebApplicationContext
org.springframework.boot.web.servlet.context.ServletWebServerApplicationContext.ExistingWebApplicationScopes

org.springframework.boot.web.reactive.context.ReactiveWebApplicationContext
    + org.springframework.boot.web.reactive.context.ConfigurableReactiveWebApplicationContext
        + org.springframework.boot.web.reactive.context.AnnotationConfigReactiveWebApplicationContext
        + org.springframework.boot.test.context.assertj.AssertableReactiveWebApplicationContext
        + org.springframework.boot.web.reactive.context.GenericReactiveWebApplicationContext
            + org.springframework.boot.web.reactive.context.ReactiveWebServerApplicationContext
                + org.springframework.boot.web.reactive.context.AnnotationConfigReactiveWebServerApplicationContext

org.springframework.boot.web.context.WebServerInitializedEvent
    + org.springframework.boot.web.servlet.context.ServletWebServerInitializedEvent
    + org.springframework.boot.web.reactive.context.ReactiveWebServerInitializedEvent


org.springframework.boot.web.context.WebServerPortFileWriter
org.springframework.boot.web.context.WebServerGracefulShutdownLifecycle

org.springframework.boot.web.client.RestTemplateBuilder
org.springframework.boot.web.client.RestTemplateRequestCustomizer
org.springframework.boot.web.client.ClientHttpRequestFactorySupplier

org.springframework.boot.web.client.RestTemplateCustomizer
    + org.springframework.boot.actuate.metrics.web.client.MetricsRestTemplateCustomizer
    + org.springframework.boot.test.web.client.MockServerRestTemplateCustomizer

org.springframework.boot.web.client.RootUriTemplateHandler
    + org.springframework.boot.test.web.client.LocalHostUriTemplateHandler

org.springframework.boot.web.codec.CodecCustomizer

org.springframework.boot.web.error.ErrorAttributeOptions
org.springframework.boot.web.error.ErrorAttributeOptions.Include

org.springframework.boot.web.servlet.filter.OrderedFilter
    + org.springframework.boot.web.servlet.filter.OrderedFormContentFilter
    + org.springframework.boot.web.servlet.filter.OrderedHiddenHttpMethodFilter
    + org.springframework.boot.web.servlet.filter.OrderedRequestContextFilter
    + org.springframework.boot.web.servlet.filter.OrderedCharacterEncodingFilter

org.springframework.boot.web.servlet.filter.ApplicationContextHeaderFilter
org.springframework.boot.web.servlet.filter.ErrorPageSecurityFilter

org.springframework.boot.web.reactive.filter.OrderedWebFilter
    + org.springframework.boot.web.reactive.filter.OrderedHiddenHttpMethodFilter

org.springframework.boot.web.servlet.error.ErrorAttributes
    + org.springframework.boot.web.servlet.error.DefaultErrorAttributes

org.springframework.boot.web.servlet.error.ErrorController
    + org.springframework.boot.autoconfigure.web.servlet.error.AbstractErrorController
        + org.springframework.boot.autoconfigure.web.servlet.error.BasicErrorController

org.springframework.boot.web.reactive.error.ErrorAttributes
    + org.springframework.boot.web.reactive.error.DefaultErrorAttributes

org.springframework.boot.web.reactive.error.ErrorWebExceptionHandler
    + org.springframework.boot.autoconfigure.web.reactive.error.AbstractErrorWebExceptionHandler
        + org.springframework.boot.autoconfigure.web.reactive.error.DefaultErrorWebExceptionHandler

org.springframework.boot.web.servlet.ServletContextInitializer
    + org.springframework.boot.actuate.endpoint.web.ServletEndpointRegistrar
    + org.springframework.boot.web.servlet.RegistrationBean
        + org.springframework.boot.web.servlet.ServletListenerRegistrationBean<T>
        + org.springframework.boot.web.servlet.DynamicRegistrationBean<D>
            + org.springframework.boot.web.servlet.AbstractFilterRegistrationBean<T>
                + org.springframework.boot.web.servlet.DelegatingFilterProxyRegistrationBean
                + org.springframework.boot.web.servlet.FilterRegistrationBean<T>
            + org.springframework.boot.web.servlet.ServletRegistrationBean<T>
                + org.springframework.boot.autoconfigure.web.servlet.DispatcherServletRegistrationBean

org.springframework.boot.web.servlet.DispatcherType
org.springframework.boot.web.servlet.MultipartConfigFactory
org.springframework.boot.web.servlet.ServletComponentScan
org.springframework.boot.web.servlet.ServletContextInitializerBeans
org.springframework.boot.web.servlet.ServletContextInitializerBeans.RegistrationBeanAdapter
org.springframework.boot.web.servlet.WebListenerRegistrar

org.springframework.boot.web.servlet.server.Jsp
org.springframework.boot.web.servlet.server.Encoding
org.springframework.boot.web.servlet.server.Encoding.Type
org.springframework.boot.web.servlet.server.CookieSameSiteSupplier
org.springframework.boot.web.servlet.support.SpringBootServletInitializer
org.springframework.boot.web.servlet.context.WebApplicationContextServletContextAwareProcessor
org.springframework.boot.web.servlet.view.MustacheView
org.springframework.boot.web.servlet.view.MustacheViewResolver

org.springframework.boot.web.reactive.context.ConfigurableReactiveWebEnvironment
    + org.springframework.boot.web.reactive.context.StandardReactiveWebEnvironment

org.springframework.boot.web.reactive.function.client.WebClientCustomizer
org.springframework.boot.web.reactive.result.view.MustacheView
org.springframework.boot.web.reactive.result.view.MustacheViewResolver













