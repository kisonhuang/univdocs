# web

## WebApplicationInitializer

```java
org.springframework.web.WebApplicationInitializer
    + org.springframework.web.context.AbstractContextLoaderInitializer
        + org.springframework.web.servlet.support.AbstractDispatcherServletInitializer
            + org.springframework.web.servlet.support.AbstractAnnotationConfigDispatcherServletInitializer
    + org.springframework.web.server.adapter.AbstractReactiveWebInitializer
```

## ContextLoader

```java
org.springframework.web.context.ContextLoader
    + org.springframework.web.context.ContextLoaderListener
```

## MultipartFile

```java
org.springframework.web.multipart.MultipartFile
    + org.springframework.web.multipart.commons.CommonsMultipartFile
    + org.springframework.mock.web.MockMultipartFile
```

## MultipartRequest

```java
org.springframework.web.multipart.MultipartRequest
    + org.springframework.web.multipart.MultipartHttpServletRequest
        + org.springframework.web.multipart.support.AbstractMultipartHttpServletRequest
            + org.springframework.web.multipart.support.DefaultMultipartHttpServletRequest
            + org.springframework.web.multipart.support.StandardMultipartHttpServletRequest
        + org.springframework.mock.web.MockMultipartHttpServletRequest
```

## MultipartResolver

```java
org.springframework.web.multipart.MultipartResolver
    + org.springframework.web.multipart.commons.CommonsMultipartResolver
    + org.springframework.web.multipart.support.StandardServletMultipartResolver
```

## HttpRequestHandler

```java
org.springframework.web.HttpRequestHandler
    + org.springframework.web.servlet.resource.DefaultServletHttpRequestHandler
    + org.springframework.remoting.caucho.HessianServiceExporter
    + org.springframework.remoting.httpinvoker.HttpInvokerServiceExporter
    + org.springframework.web.servlet.resource.ResourceHttpRequestHandler
    + org.springframework.web.socket.sockjs.support.SockJsHttpRequestHandler
    + org.springframework.web.socket.server.support.WebSocketHttpRequestHandler
```

## ContentNegotiationStrategy

```java
org.springframework.web.accept.ContentNegotiationStrategy
    + org.springframework.web.accept.AbstractMappingContentNegotiationStrategy
        + org.springframework.web.accept.ParameterContentNegotiationStrategy
        + org.springframework.web.accept.PathExtensionContentNegotiationStrategy
            + org.springframework.web.accept.ServletPathExtensionContentNegotiationStrategy
    + org.springframework.web.accept.ContentNegotiationManager
    + org.springframework.web.accept.FixedContentNegotiationStrategy
    + org.springframework.web.accept.HeaderContentNegotiationStrategy
```

## MediaTypeFileExtensionResolver

```java
org.springframework.web.accept.MediaTypeFileExtensionResolver
    + org.springframework.web.accept.ContentNegotiationManager
    + org.springframework.web.accept.MappingMediaTypeFileExtensionResolver
        + org.springframework.web.accept.AbstractMappingContentNegotiationStrategy
            + org.springframework.web.accept.ParameterContentNegotiationStrategy
            + org.springframework.web.accept.PathExtensionContentNegotiationStrategy
                + org.springframework.web.accept.ServletPathExtensionContentNegotiationStrategy
```

## ValueConstants

```java
org.springframework.web.bind.annotation.ValueConstants
```

## SessionAttributeStore

```java
org.springframework.web.bind.support.SessionAttributeStore
    + org.springframework.web.bind.support.DefaultSessionAttributeStore
```

## SessionStatus

```java
org.springframework.web.bind.support.SessionStatus
    + org.springframework.web.bind.support.SimpleSessionStatus
```

## WebArgumentResolver

```java
org.springframework.web.bind.support.WebArgumentResolver
```

## WebBindingInitializer

```java
org.springframework.web.bind.support.WebBindingInitializer
    + org.springframework.web.bind.support.ConfigurableWebBindingInitializer
```

## WebDataBinderFactory

```java
org.springframework.web.bind.support.WebDataBinderFactory
    + org.springframework.web.bind.support.DefaultDataBinderFactory
        + org.springframework.web.method.annotation.InitBinderDataBinderFactory
            + org.springframework.web.servlet.mvc.method.annotation.ServletRequestDataBinderFactory
```

## AsyncRequestCallback

```java
org.springframework.web.client.AsyncRequestCallback
```

## AsyncRestOperations

```java
org.springframework.web.client.AsyncRestOperations
    + org.springframework.web.client.AsyncRestTemplate
```

## RequestCallback

```java
org.springframework.web.client.RequestCallback
```

## ResponseErrorHandler

```java
org.springframework.web.client.ResponseErrorHandler
    + org.springframework.web.client.DefaultResponseErrorHandler
        + org.springframework.web.client.ExtractingResponseErrorHandler
```

## ResponseExtractor

```java
org.springframework.web.client.ResponseExtractor<T>
    + org.springframework.web.client.HttpMessageConverterExtractor<T>
```

## WebRequestInterceptor

```java
org.springframework.web.context.request.WebRequestInterceptor
    + org.springframework.web.context.request.AsyncWebRequestInterceptor
        + org.springframework.orm.jpa.support.OpenEntityManagerInViewInterceptor
        + org.springframework.orm.hibernate5.support.OpenSessionInViewInterceptor
```

## RequestAttributes

```java
org.springframework.web.context.request.RequestAttributes
    + org.springframework.web.context.request.AbstractRequestAttributes
        + org.springframework.web.context.request.ServletRequestAttributes
            + org.springframework.web.context.request.ServletWebRequest
                + org.springframework.web.servlet.handler.DispatcherServletWebRequest
                + org.springframework.web.context.request.async.StandardServletAsyncWebRequest
    + org.springframework.web.context.request.FacesRequestAttributes
        + org.springframework.web.context.request.FacesWebRequest
    + org.springframework.web.context.request.WebRequest
        + org.springframework.web.context.request.NativeWebRequest
            + org.springframework.web.context.request.FacesWebRequest
            + org.springframework.web.context.request.ServletWebRequest
                + org.springframework.web.servlet.handler.DispatcherServletWebRequest
                + org.springframework.web.context.request.async.StandardServletAsyncWebRequest
            + org.springframework.web.context.request.async.AsyncWebRequest
                + org.springframework.web.context.request.async.StandardServletAsyncWebRequest
```

## CallableProcessingInterceptor

```java
org.springframework.web.context.request.async.CallableProcessingInterceptor
    + org.springframework.web.context.request.async.CallableProcessingInterceptorAdapter
    + org.springframework.web.context.request.async.TimeoutCallableProcessingInterceptor
```

## DeferredResultHandler

```java
org.springframework.web.context.request.async.DeferredResult.DeferredResultHandler
```

## DeferredResultProcessingInterceptor

```java
org.springframework.web.context.request.async.DeferredResultProcessingInterceptor
    + org.springframework.web.context.request.async.DeferredResultProcessingInterceptorAdapter
    + org.springframework.web.context.request.async.TimeoutDeferredResultProcessingInterceptor
```

## CorsConfigurationSource

```java
org.springframework.web.cors.CorsConfigurationSource
    + org.springframework.web.socket.sockjs.support.AbstractSockJsService
        + org.springframework.web.socket.sockjs.transport.TransportHandlingSockJsService
            + org.springframework.web.socket.sockjs.transport.handler.DefaultSockJsService
    + org.springframework.web.servlet.handler.HandlerMappingIntrospector
    + org.springframework.web.servlet.resource.ResourceHttpRequestHandler
    + org.springframework.web.socket.sockjs.support.SockJsHttpRequestHandler
    + org.springframework.web.cors.UrlBasedCorsConfigurationSource
```

## CorsProcessor

```java
org.springframework.web.cors.CorsProcessor
    + org.springframework.web.cors.DefaultCorsProcessor
```

## CorsConfigurationSource

```java
org.springframework.web.cors.reactive.CorsConfigurationSource
    + org.springframework.web.cors.reactive.UrlBasedCorsConfigurationSource
```

## CorsProcessor

```java
org.springframework.web.cors.reactive.CorsProcessor
    + org.springframework.web.cors.reactive.DefaultCorsProcessor
```

## PreFlightRequestHandler

```java
org.springframework.web.cors.reactive.PreFlightRequestHandler
    + org.springframework.web.reactive.DispatcherHandler
```

## HandlerMethodReturnValueHandler

```java
org.springframework.web.method.support.HandlerMethodReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.AbstractMessageConverterMethodProcessor
        + org.springframework.web.servlet.mvc.method.annotation.HttpEntityMethodProcessor
        + org.springframework.web.servlet.mvc.method.annotation.RequestResponseBodyMethodProcessor
    + org.springframework.web.servlet.mvc.method.annotation.AsyncTaskMethodReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.CallableMethodReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.DeferredResultMethodReturnValueHandler
    + org.springframework.web.method.support.HandlerMethodReturnValueHandlerComposite
    + org.springframework.web.servlet.mvc.method.annotation.HttpHeadersReturnValueHandler
    + org.springframework.web.method.annotation.MapMethodProcessor
    + org.springframework.web.servlet.mvc.method.annotation.ModelAndViewMethodReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.ModelAndViewResolverMethodReturnValueHandler
    + org.springframework.web.method.annotation.ModelAttributeMethodProcessor
        + org.springframework.web.servlet.mvc.method.annotation.ServletModelAttributeMethodProcessor
    + org.springframework.web.method.annotation.ModelMethodProcessor
    + org.springframework.web.servlet.mvc.method.annotation.ResponseBodyEmitterReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.StreamingResponseBodyReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.ViewMethodReturnValueHandler
    + org.springframework.web.servlet.mvc.method.annotation.ViewNameMethodReturnValueHandler
    + org.springframework.web.method.support.AsyncHandlerMethodReturnValueHandler
```

## HandlerMethodArgumentResolver

```java
org.springframework.web.method.support.HandlerMethodArgumentResolver
    + org.springframework.web.servlet.mvc.method.annotation.AbstractMessageConverterMethodArgumentResolver
        + org.springframework.web.servlet.mvc.method.annotation.AbstractMessageConverterMethodProcessor
            + org.springframework.web.servlet.mvc.method.annotation.HttpEntityMethodProcessor
            + org.springframework.web.servlet.mvc.method.annotation.RequestResponseBodyMethodProcessor
        + org.springframework.web.servlet.mvc.method.annotation.RequestPartMethodArgumentResolver
    + org.springframework.web.method.annotation.AbstractNamedValueMethodArgumentResolver
        + org.springframework.web.method.annotation.AbstractCookieValueMethodArgumentResolver
            + org.springframework.web.servlet.mvc.method.annotation.ServletCookieValueMethodArgumentResolver
        + org.springframework.web.method.annotation.ExpressionValueMethodArgumentResolver
        + org.springframework.web.servlet.mvc.method.annotation.MatrixVariableMethodArgumentResolver
        + org.springframework.web.servlet.mvc.method.annotation.PathVariableMethodArgumentResolver
        + org.springframework.web.servlet.mvc.method.annotation.RequestAttributeMethodArgumentResolver
        + org.springframework.web.method.annotation.RequestHeaderMethodArgumentResolver
        + org.springframework.web.method.annotation.RequestParamMethodArgumentResolver
        + org.springframework.web.servlet.mvc.method.annotation.SessionAttributeMethodArgumentResolver
    + org.springframework.web.method.annotation.AbstractWebArgumentResolverAdapter
        + org.springframework.web.servlet.mvc.method.annotation.ServletWebArgumentResolverAdapter
    + org.springframework.web.servlet.mvc.method.annotation.ContinuationHandlerMethodArgumentResolver
    + org.springframework.web.method.annotation.ErrorsMethodArgumentResolver
    + org.springframework.web.method.support.HandlerMethodArgumentResolverComposite
    + org.springframework.web.method.annotation.MapMethodProcessor
    + org.springframework.web.servlet.mvc.method.annotation.MatrixVariableMapMethodArgumentResolver
    + org.springframework.web.method.annotation.ModelAttributeMethodProcessor
        + org.springframework.web.servlet.mvc.method.annotation.ServletModelAttributeMethodProcessor
    + org.springframework.web.method.annotation.ModelMethodProcessor
    + org.springframework.web.servlet.mvc.method.annotation.PathVariableMapMethodArgumentResolver
    + org.springframework.web.servlet.mvc.method.annotation.PrincipalMethodArgumentResolver
    + org.springframework.web.servlet.mvc.method.annotation.RedirectAttributesMethodArgumentResolver
    + org.springframework.web.method.annotation.RequestHeaderMapMethodArgumentResolver
    + org.springframework.web.method.annotation.RequestParamMapMethodArgumentResolver
    + org.springframework.web.servlet.mvc.method.annotation.ServletRequestMethodArgumentResolver
    + org.springframework.web.servlet.mvc.method.annotation.ServletResponseMethodArgumentResolver
    + org.springframework.web.method.annotation.SessionStatusMethodArgumentResolver
    + org.springframework.web.servlet.mvc.method.annotation.UriComponentsBuilderMethodArgumentResolver
```

## UriComponentsContributor

```java
org.springframework.web.method.support.UriComponentsContributor
    + org.springframework.web.method.support.CompositeUriComponentsContributor
    + org.springframework.web.servlet.mvc.method.annotation.PathVariableMethodArgumentResolver
    + org.springframework.web.method.annotation.RequestParamMethodArgumentResolver
```

## LocaleContextResolver

```java
org.springframework.web.server.i18n.LocaleContextResolver
    + org.springframework.web.server.i18n.AcceptHeaderLocaleContextResolver
    + org.springframework.web.server.i18n.FixedLocaleContextResolver
```

## ServerWebExchange

```java
org.springframework.web.server.ServerWebExchange
    + org.springframework.web.server.adapter.DefaultServerWebExchange
        + org.springframework.mock.web.server.MockServerWebExchange
    + org.springframework.web.server.ServerWebExchangeDecorator

org.springframework.web.server.ServerWebExchange.Builder
```

## WebExceptionHandler

```java
org.springframework.web.server.WebExceptionHandler
    + org.springframework.web.server.handler.ResponseStatusExceptionHandler
        + org.springframework.web.reactive.handler.WebFluxResponseStatusExceptionHandler
```

## WebFilter

```java
org.springframework.web.server.WebFilter
    + org.springframework.web.cors.reactive.CorsWebFilter
    + org.springframework.web.filter.reactive.ForwardedHeaderFilter
    + org.springframework.web.filter.reactive.HiddenHttpMethodFilter
    + org.springframework.web.cors.reactive.PreFlightRequestWebFilter
    + org.springframework.web.filter.reactive.ServerWebExchangeContextFilter
```

## WebFilterChain

```java
org.springframework.web.server.WebFilterChain
    + org.springframework.web.server.handler.DefaultWebFilterChain
```

## WebHandler

```java
org.springframework.web.server.WebHandler
    + org.springframework.web.reactive.DispatcherHandler
    + org.springframework.web.reactive.resource.ResourceWebHandler
    + org.springframework.web.server.handler.WebHandlerDecorator
        + org.springframework.web.server.handler.ExceptionHandlingWebHandler
        + org.springframework.web.server.handler.FilteringWebHandler
        + org.springframework.web.server.adapter.HttpWebHandlerAdapter
```

## WebSession

```java
org.springframework.web.server.WebSession
    + org.springframework.mock.web.server.MockWebSession
```

## WebSessionIdResolver

```java
org.springframework.web.server.session.WebSessionIdResolver
    + org.springframework.web.server.session.CookieWebSessionIdResolver
    + org.springframework.web.server.session.HeaderWebSessionIdResolver
```

## WebSessionManager

```java
org.springframework.web.server.session.WebSessionManager
    + org.springframework.web.server.session.DefaultWebSessionManager
```

## WebSessionStore

```java
org.springframework.web.server.session.WebSessionStore
    + org.springframework.web.server.session.InMemoryWebSessionStore
```

## UriBuilder

```java
org.springframework.web.util.UriBuilder
    + org.springframework.web.util.UriComponentsBuilder
    + org.springframework.web.servlet.support.ServletUriComponentsBuilder
```

## UriTemplateHandler

```java
org.springframework.web.util.UriTemplateHandler
    + org.springframework.web.util.AbstractUriTemplateHandler
        + org.springframework.web.util.DefaultUriTemplateHandler
    + org.springframework.web.util.UriBuilderFactory
        + org.springframework.web.util.DefaultUriBuilderFactory
```

## UriTemplateVariables

```java
org.springframework.web.util.UriComponents.UriTemplateVariables
```

## ConfigurableWebEnvironment

```java
org.springframework.web.context.ConfigurableWebEnvironment
    + org.springframework.web.context.support.StandardServletEnvironment
```

## ServletContextAware

```java
org.springframework.web.context.ServletConfigAware
org.springframework.web.context.ServletContextAware
```

## WebApplicationContext

```java
org.springframework.web.context.WebApplicationContext
    + org.springframework.web.context.ConfigurableWebApplicationContext
        + org.springframework.web.context.support.AbstractRefreshableWebApplicationContext
            + org.springframework.web.context.support.AnnotationConfigWebApplicationContext
            + org.springframework.web.context.support.GroovyWebApplicationContext
            + org.springframework.web.context.support.XmlWebApplicationContext
        + org.springframework.web.context.support.GenericWebApplicationContext
        + org.springframework.web.context.support.StaticWebApplicationContext
```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```

## 

```java

```



































