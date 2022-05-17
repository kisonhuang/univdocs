# web

## 注解

```java
org.springframework.web.bind.annotation.RestController

org.springframework.web.bind.annotation.ControllerAdvice
org.springframework.web.bind.annotation.RestControllerAdvice
org.springframework.web.bind.annotation.ExceptionHandler

org.springframework.web.bind.annotation.RequestMapping
org.springframework.web.bind.annotation.GetMapping
org.springframework.web.bind.annotation.PostMapping
org.springframework.web.bind.annotation.PutMapping
org.springframework.web.bind.annotation.PatchMapping
org.springframework.web.bind.annotation.DeleteMapping
org.springframework.web.bind.annotation.Mapping

org.springframework.web.bind.annotation.PathVariable
org.springframework.web.bind.annotation.RequestAttribute
org.springframework.web.bind.annotation.RequestParam
org.springframework.web.bind.annotation.RequestHeader
org.springframework.web.bind.annotation.RequestBody
org.springframework.web.bind.annotation.RequestPart

org.springframework.web.bind.annotation.ResponseBody
org.springframework.web.bind.annotation.ResponseStatus

org.springframework.web.bind.annotation.CookieValue
org.springframework.web.bind.annotation.SessionAttribute
org.springframework.web.bind.annotation.SessionAttributes

org.springframework.web.bind.annotation.InitBinder
org.springframework.web.bind.annotation.ModelAttribute
org.springframework.web.bind.annotation.MatrixVariable
org.springframework.web.bind.annotation.CrossOrigin

org.springframework.web.context.annotation.ApplicationScope
org.springframework.web.context.annotation.RequestScope
org.springframework.web.context.annotation.SessionScope
```

## 枚举

```
org.springframework.web.bind.annotation.RequestMethod
org.springframework.web.util.pattern.PatternParseException.PatternMessage
```

## SpringServletContainerInitializer

```java
org.springframework.web.SpringServletContainerInitializer
```

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

## HttpServletBean

```java
org.springframework.web.servlet.HttpServletBean
    + org.springframework.web.servlet.FrameworkServlet
        + org.springframework.web.servlet.DispatcherServlet
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

## ServletContextResource

```java
org.springframework.web.context.support.ServletContextResource
org.springframework.web.context.support.ServletContextResourceLoader
org.springframework.web.context.support.ServletContextResourcePatternResolver
```

## ConfigurableWebEnvironment

```java
org.springframework.web.context.ConfigurableWebEnvironment
    + org.springframework.web.context.support.StandardServletEnvironment
```

## Listener

```java
org.springframework.web.context.ContextCleanupListener
org.springframework.web.context.request.RequestContextListener
org.springframework.web.context.request.DestructionCallbackBindingListener
org.springframework.web.util.WebAppRootListener
org.springframework.web.util.HttpSessionMutexListener
org.springframework.web.util.IntrospectorCleanupListener
org.springframework.web.context.support.RequestHandledEvent
org.springframework.web.context.support.ServletRequestHandledEvent
```

## ServletContext

```java
org.springframework.web.context.support.ServletContextParameterFactoryBean
org.springframework.web.context.support.ServletContextAttributeFactoryBean
org.springframework.web.context.support.ServletContextAttributeExporter
org.springframework.web.context.support.ServletContextAwareProcessor
org.springframework.web.context.support.ServletContextLiveBeansView
org.springframework.web.context.support.ServletContextPropertySource
```

## Scope

```java
org.springframework.web.context.support.ServletContextScope
org.springframework.web.context.request.AbstractRequestAttributesScope
org.springframework.web.context.request.RequestScope
org.springframework.web.context.request.SessionScope
```

## Filter

```java
org.springframework.web.filter.AbstractRequestLoggingFilter
org.springframework.web.filter.CharacterEncodingFilter
org.springframework.web.filter.CommonsRequestLoggingFilter
org.springframework.web.filter.CompositeFilter
org.springframework.web.filter.CorsFilter
org.springframework.web.filter.DelegatingFilterProxy
org.springframework.web.filter.FormContentFilter
org.springframework.web.filter.ForwardedHeaderFilter
org.springframework.web.filter.GenericFilterBean
org.springframework.web.filter.HiddenHttpMethodFilter
org.springframework.web.filter.HttpPutFormContentFilter
org.springframework.web.filter.OncePerRequestFilter
org.springframework.web.filter.RelativeRedirectFilter
org.springframework.web.filter.RequestContextFilter
org.springframework.web.filter.ServletContextRequestLoggingFilter
org.springframework.web.filter.ServletRequestPathFilter
org.springframework.web.filter.ShallowEtagHeaderFilter
org.springframework.web.multipart.support.MultipartFilter
```

## Utils

```java
org.springframework.web.bind.ServletRequestUtils
org.springframework.web.context.request.async.WebAsyncUtils
org.springframework.web.context.support.WebApplicationContextUtils
org.springframework.web.cors.CorsUtils
org.springframework.web.cors.reactive.CorsUtils
org.springframework.web.jsf.FacesContextUtils
org.springframework.web.multipart.support.StandardServletPartUtils
org.springframework.web.util.HtmlUtils
org.springframework.web.util.JavaScriptUtils
org.springframework.web.util.ServletContextPropertyUtils
org.springframework.web.util.TagUtils
org.springframework.web.util.WebUtils
```

## Exception

```java
org.springframework.web.multipart.MultipartException
    + org.springframework.web.multipart.MaxUploadSizeExceededException

org.springframework.web.server.ResponseStatusException
    + org.springframework.web.server.MediaTypeNotSupportedStatusException
    + org.springframework.web.server.MethodNotAllowedException
    + org.springframework.web.server.NotAcceptableStatusException
    + org.springframework.web.server.ServerErrorException
    + org.springframework.web.server.ServerWebInputException
        + org.springframework.web.bind.support.WebExchangeBindException
    + org.springframework.web.server.UnsupportedMediaTypeStatusException

+ org.springframework.web.client.RestClientException
    + org.springframework.web.client.ResourceAccessException
    + org.springframework.web.client.RestClientResponseException
        + org.springframework.web.client.HttpStatusCodeException
            + org.springframework.web.client.HttpClientErrorException
                + org.springframework.web.client.HttpClientErrorException.BadRequest
                + org.springframework.web.client.HttpClientErrorException.Conflict
                + org.springframework.web.client.HttpClientErrorException.Forbidden
                + org.springframework.web.client.HttpClientErrorException.Gone
                + org.springframework.web.client.HttpClientErrorException.MethodNotAllowed
                + org.springframework.web.client.HttpClientErrorException.NotAcceptable
                + org.springframework.web.client.HttpClientErrorException.NotFound
                + org.springframework.web.client.HttpClientErrorException.TooManyRequests
                + org.springframework.web.client.HttpClientErrorException.Unauthorized
                + org.springframework.web.client.HttpClientErrorException.UnprocessableEntity
                + org.springframework.web.client.HttpClientErrorException.UnsupportedMediaType
            + org.springframework.web.client.HttpServerErrorException
                + org.springframework.web.client.HttpServerErrorException.BadGateway
                + org.springframework.web.client.HttpServerErrorException.GatewayTimeout
                + org.springframework.web.client.HttpServerErrorException.InternalServerError
                + org.springframework.web.client.HttpServerErrorException.NotImplemented
                + org.springframework.web.client.HttpServerErrorException.ServiceUnavailable
        + org.springframework.web.client.UnknownHttpStatusCodeException
    + org.springframework.web.client.UnknownContentTypeException

org.springframework.web.HttpMediaTypeException
    + org.springframework.web.HttpMediaTypeNotAcceptableException
    + org.springframework.web.HttpMediaTypeNotSupportedException

org.springframework.web.util.NestedServletException
    + org.springframework.web.bind.ServletRequestBindingException
        + org.springframework.web.bind.MissingRequestValueException
            + org.springframework.web.bind.MissingMatrixVariableException
            + org.springframework.web.bind.MissingPathVariableException
            + org.springframework.web.bind.MissingRequestCookieException
            + org.springframework.web.bind.MissingRequestHeaderException
            + org.springframework.web.bind.MissingServletRequestParameterException
        + org.springframework.web.bind.UnsatisfiedServletRequestParameterException

org.springframework.web.bind.EscapedErrors
org.springframework.web.bind.MethodArgumentNotValidException
org.springframework.web.context.request.async.AsyncRequestTimeoutException
org.springframework.web.HttpRequestMethodNotSupportedException
org.springframework.web.HttpSessionRequiredException
org.springframework.web.method.annotation.MethodArgumentConversionNotSupportedException
org.springframework.web.method.annotation.MethodArgumentTypeMismatchException
org.springframework.web.multipart.support.MissingServletRequestPartException
org.springframework.web.util.pattern.PatternParseException
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

## DeferredResultHandler

```java
org.springframework.web.context.request.async.DeferredResult.DeferredResultHandler
```

## DeferredResultProcessingInterceptor

```java
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

## ServletContextAware

```java
org.springframework.web.context.ServletConfigAware
org.springframework.web.context.ServletContextAware
```

## WebDataBinder

```java
org.springframework.web.bind.WebDataBinder
    + org.springframework.web.bind.ServletRequestDataBinder
        + org.springframework.web.servlet.mvc.method.annotation.ExtendedServletRequestDataBinder
    + org.springframework.web.bind.support.WebExchangeDataBinder
    + org.springframework.web.bind.support.WebRequestDataBinder
```

## ServletRequestPathUtils

```java
org.springframework.web.util.ServletRequestPathUtils
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





org.springframework.web.bind.ServletRequestParameterPropertyValues
org.springframework.web.bind.support.SpringWebConstraintValidatorFactory
org.springframework.web.client.support.RestGatewaySupport
org.springframework.web.context.request.async.DeferredResult
org.springframework.web.context.request.async.WebAsyncManager
org.springframework.web.context.request.async.WebAsyncTask
org.springframework.web.context.request.RequestContextHolder
org.springframework.web.context.support.ContextExposingHttpServletRequest
org.springframework.web.context.support.HttpRequestHandlerServlet
org.springframework.web.context.support.LiveBeansViewServlet
org.springframework.web.context.support.ServletConfigPropertySource
org.springframework.web.context.support.SpringBeanAutowiringSupport
org.springframework.web.context.support.WebApplicationObjectSupport
org.springframework.web.jsf.DecoratingNavigationHandler
org.springframework.web.jsf.DelegatingNavigationHandlerProxy
org.springframework.web.jsf.DelegatingPhaseListenerMulticaster
org.springframework.web.jsf.el.SpringBeanFacesELResolver
org.springframework.web.jsf.el.WebApplicationContextFacesELResolver
org.springframework.web.method.annotation.AbstractNamedValueMethodArgumentResolver.NamedValueInfo
org.springframework.web.method.annotation.ExceptionHandlerMethodResolver
org.springframework.web.method.annotation.ModelFactory
org.springframework.web.method.annotation.SessionAttributesHandler
org.springframework.web.method.ControllerAdviceBean
org.springframework.web.method.HandlerMethod
org.springframework.web.method.HandlerTypePredicate
org.springframework.web.method.HandlerTypePredicate.Builder
org.springframework.web.method.support.InvocableHandlerMethod

org.springframework.web.multipart.commons.CommonsFileUploadSupport
org.springframework.web.multipart.commons.CommonsFileUploadSupport.MultipartParsingResult
org.springframework.web.multipart.support.ByteArrayMultipartFileEditor
org.springframework.web.multipart.support.MultipartResolutionDelegate
org.springframework.web.multipart.support.StringMultipartFileEditor
org.springframework.web.server.adapter.ForwardedHeaderTransformer
org.springframework.web.server.adapter.WebHttpHandlerBuilder
org.springframework.web.server.adapter.WebHttpHandlerBuilder.SpringWebBlockHoundIntegration
org.springframework.web.util.ContentCachingRequestWrapper
org.springframework.web.util.ContentCachingResponseWrapper
















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



































