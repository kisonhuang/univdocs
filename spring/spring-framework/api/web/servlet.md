# servlet

## HandlerInterceptor

```java
org.springframework.web.servlet.HandlerInterceptor
    + org.springframework.web.servlet.handler.ConversionServiceExposingInterceptor
    + org.springframework.web.servlet.i18n.LocaleChangeInterceptor
    + org.springframework.web.servlet.handler.MappedInterceptor
    + org.springframework.web.servlet.resource.ResourceUrlProviderExposingInterceptor
    + org.springframework.web.servlet.theme.ThemeChangeInterceptor
    + org.springframework.web.servlet.handler.UserRoleAuthorizationInterceptor
    + org.springframework.web.servlet.mvc.WebContentInterceptor
    + org.springframework.web.servlet.AsyncHandlerInterceptor
        + org.springframework.web.servlet.handler.HandlerInterceptorAdapter
        + org.springframework.web.servlet.handler.WebRequestHandlerInterceptorAdapter
```

## FlashMapManager

```java
org.springframework.web.servlet.FlashMapManager
    + org.springframework.web.servlet.support.AbstractFlashMapManager
        + org.springframework.web.servlet.support.SessionFlashMapManager
```

## HandlerAdapter

```java
org.springframework.web.servlet.HandlerAdapter
    + org.springframework.web.servlet.mvc.method.AbstractHandlerMethodAdapter
        + org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter
    + org.springframework.web.servlet.function.support.HandlerFunctionAdapter
    + org.springframework.web.servlet.mvc.HttpRequestHandlerAdapter
    + org.springframework.web.servlet.mvc.SimpleControllerHandlerAdapter
    + org.springframework.web.servlet.handler.SimpleServletHandlerAdapter
```

## HandlerExceptionResolver

```java
org.springframework.web.servlet.HandlerExceptionResolver
    + org.springframework.web.servlet.handler.AbstractHandlerExceptionResolver
        + org.springframework.web.servlet.handler.AbstractHandlerMethodExceptionResolver
            + org.springframework.web.servlet.mvc.method.annotation.ExceptionHandlerExceptionResolver
        + org.springframework.web.servlet.mvc.support.DefaultHandlerExceptionResolver
        + org.springframework.web.servlet.mvc.annotation.ResponseStatusExceptionResolver
        + org.springframework.web.servlet.handler.SimpleMappingExceptionResolver
    + org.springframework.web.servlet.handler.HandlerExceptionResolverComposite
```

## HandlerMapping

```java
org.springframework.web.servlet.HandlerMapping
    + org.springframework.web.servlet.handler.AbstractHandlerMapping
        + org.springframework.web.servlet.handler.AbstractHandlerMethodMapping<T>
            + org.springframework.web.servlet.mvc.method.RequestMappingInfoHandlerMapping
                + org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping
        + org.springframework.web.servlet.handler.AbstractUrlHandlerMapping
            + org.springframework.web.servlet.handler.AbstractDetectingUrlHandlerMapping
                + org.springframework.web.servlet.handler.BeanNameUrlHandlerMapping
            + org.springframework.web.servlet.handler.SimpleUrlHandlerMapping
                + org.springframework.web.socket.server.support.WebSocketHandlerMapping
        + org.springframework.web.servlet.function.support.RouterFunctionMapping
    + org.springframework.web.servlet.handler.MatchableHandlerMapping
        + org.springframework.web.servlet.handler.AbstractUrlHandlerMapping
            + org.springframework.web.servlet.handler.AbstractDetectingUrlHandlerMapping
                + org.springframework.web.servlet.handler.BeanNameUrlHandlerMapping
            + org.springframework.web.servlet.handler.SimpleUrlHandlerMapping
                + org.springframework.web.socket.server.support.WebSocketHandlerMapping
        + org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping
```

## LocaleResolver

```java
org.springframework.web.servlet.LocaleResolver
    + org.springframework.web.servlet.i18n.AbstractLocaleResolver
        + org.springframework.web.servlet.i18n.AbstractLocaleContextResolver
            + org.springframework.web.servlet.i18n.FixedLocaleResolver
            + org.springframework.web.servlet.i18n.SessionLocaleResolver
    + org.springframework.web.servlet.i18n.AcceptHeaderLocaleResolver
    + org.springframework.web.servlet.LocaleContextResolver
        + org.springframework.web.servlet.i18n.AbstractLocaleContextResolver
            + org.springframework.web.servlet.i18n.FixedLocaleResolver
            + org.springframework.web.servlet.i18n.SessionLocaleResolver
        + org.springframework.web.servlet.i18n.CookieLocaleResolver
```

## RequestToViewNameTranslator

```java
org.springframework.web.servlet.RequestToViewNameTranslator
    + org.springframework.web.servlet.view.DefaultRequestToViewNameTranslator
```

## View

```java
org.springframework.web.servlet.View
    + org.springframework.web.servlet.view.AbstractView
        + org.springframework.web.servlet.view.feed.AbstractFeedView<T>
            + org.springframework.web.servlet.view.feed.AbstractAtomFeedView
            + org.springframework.web.servlet.view.feed.AbstractRssFeedView
        + org.springframework.web.servlet.view.json.AbstractJackson2View
            + org.springframework.web.servlet.view.json.MappingJackson2JsonView
            + org.springframework.web.servlet.view.xml.MappingJackson2XmlView
        + org.springframework.web.servlet.view.document.AbstractPdfView
        + org.springframework.web.servlet.view.AbstractUrlBasedView
            + org.springframework.web.servlet.view.document.AbstractPdfStamperView
            + org.springframework.web.servlet.view.AbstractTemplateView
                + org.springframework.web.servlet.view.freemarker.FreeMarkerView
                + org.springframework.web.servlet.view.groovy.GroovyMarkupView
            + org.springframework.web.servlet.view.InternalResourceView
                + org.springframework.web.servlet.view.JstlView
            + org.springframework.web.servlet.view.RedirectView
            + org.springframework.web.servlet.view.script.ScriptTemplateView
            + org.springframework.web.servlet.view.tiles3.TilesView
            + org.springframework.web.servlet.view.xslt.XsltView
        + org.springframework.web.servlet.view.document.AbstractXlsView
            + org.springframework.web.servlet.view.document.AbstractXlsxView
                + org.springframework.web.servlet.view.document.AbstractXlsxStreamingView
        + org.springframework.web.servlet.view.xml.MarshallingView
    + org.springframework.web.servlet.SmartView
        + org.springframework.web.servlet.view.RedirectView
```

## ThemeResolver

```java
org.springframework.web.servlet.ThemeResolver
    + org.springframework.web.servlet.theme.AbstractThemeResolver
        + org.springframework.web.servlet.theme.FixedThemeResolver
        + org.springframework.web.servlet.theme.SessionThemeResolver
    + org.springframework.web.servlet.theme.CookieThemeResolver
```

## ViewResolver

```java
org.springframework.web.servlet.ViewResolver
    + org.springframework.web.servlet.view.AbstractCachingViewResolver
        + org.springframework.web.servlet.view.ResourceBundleViewResolver
        + org.springframework.web.servlet.view.UrlBasedViewResolver
            + org.springframework.web.servlet.view.AbstractTemplateViewResolver
                + org.springframework.web.servlet.view.freemarker.FreeMarkerViewResolver
                + org.springframework.web.servlet.view.groovy.GroovyMarkupViewResolver
            + org.springframework.web.servlet.view.InternalResourceViewResolver
            + org.springframework.web.servlet.view.script.ScriptTemplateViewResolver
            + org.springframework.web.servlet.view.tiles3.TilesViewResolver
            + org.springframework.web.servlet.view.xslt.XsltViewResolver
        + org.springframework.web.servlet.view.XmlViewResolver
    + org.springframework.web.servlet.view.BeanNameViewResolver
    + org.springframework.web.servlet.view.ContentNegotiatingViewResolver
    + org.springframework.web.servlet.view.ViewResolverComposite
```

## ModelAndViewResolver

```java
org.springframework.web.servlet.mvc.annotation.ModelAndViewResolver
```

## WebMvcConfigurer

```java
org.springframework.web.servlet.config.annotation.WebMvcConfigurer
    + org.springframework.web.servlet.config.annotation.WebMvcConfigurerAdapter
```

## ServerResponse

```java
org.springframework.web.servlet.function.ServerResponse
    + org.springframework.web.servlet.function.AsyncServerResponse
    + org.springframework.web.servlet.function.EntityResponse<T>
    + org.springframework.web.servlet.function.RenderingResponse

org.springframework.web.servlet.function.ServerResponse.BodyBuilder
org.springframework.web.servlet.function.ServerResponse.Context
org.springframework.web.servlet.function.ServerResponse.SseBuilder
org.springframework.web.servlet.function.ServerResponse.HeadersBuilder<B>

org.springframework.web.servlet.function.EntityResponse.Builder<T>

org.springframework.web.servlet.function.RenderingResponse.Builder
```

## RouterFunction

```java
org.springframework.web.servlet.function.RouterFunction<T>
org.springframework.web.servlet.function.RouterFunctions.Builder
org.springframework.web.servlet.function.RouterFunctions.Visitor

org.springframework.web.servlet.function.HandlerFunction<T>
org.springframework.web.servlet.function.HandlerFilterFunction<T,R>

org.springframework.web.servlet.function.RequestPredicate
org.springframework.web.servlet.function.RequestPredicates.Visitor

org.springframework.web.servlet.function.ServerRequest
org.springframework.web.servlet.function.ServerRequest.Builder
org.springframework.web.servlet.function.ServerRequest.Headers
```

## HandlerMethodMappingNamingStrategy

```java
org.springframework.web.servlet.handler.HandlerMethodMappingNamingStrategy<T>
    + org.springframework.web.servlet.mvc.method.RequestMappingInfoHandlerMethodMappingNamingStrategy
```

## Controller

```javaorg.springframework.web.servlet.mvc.Controller
    + org.springframework.web.servlet.mvc.AbstractController
        + org.springframework.web.servlet.mvc.AbstractUrlViewController
            + org.springframework.web.servlet.mvc.UrlFilenameViewController
        + org.springframework.web.servlet.mvc.ParameterizableViewController
        + org.springframework.web.servlet.mvc.ServletForwardingController
        + org.springframework.web.servlet.mvc.ServletWrappingController
```

## LastModified

```java
org.springframework.web.servlet.mvc.LastModified
org.springframework.web.servlet.mvc.condition.MediaTypeExpression
org.springframework.web.servlet.mvc.condition.NameValueExpression<T>
```

## RequestCondition

```java
org.springframework.web.servlet.mvc.condition.RequestCondition<T>
    + org.springframework.web.servlet.mvc.condition.AbstractRequestCondition<T>
        + org.springframework.web.servlet.mvc.condition.CompositeRequestCondition
        + org.springframework.web.servlet.mvc.condition.ConsumesRequestCondition
        + org.springframework.web.servlet.mvc.condition.HeadersRequestCondition
        + org.springframework.web.servlet.mvc.condition.ParamsRequestCondition
        + org.springframework.web.servlet.mvc.condition.PathPatternsRequestCondition
        + org.springframework.web.servlet.mvc.condition.PatternsRequestCondition
        + org.springframework.web.servlet.mvc.condition.ProducesRequestCondition
        + org.springframework.web.servlet.mvc.condition.RequestConditionHolder
        + org.springframework.web.servlet.mvc.condition.RequestMethodsRequestCondition
    + org.springframework.web.servlet.mvc.method.RequestMappingInfo
```

## RequestMappingInfo

```java
org.springframework.web.servlet.mvc.method.RequestMappingInfo.Builder
org.springframework.web.servlet.mvc.method.annotation.MvcUriComponentsBuilder.MethodInvocationInfo
```

## RequestBodyAdvice

```java
org.springframework.web.servlet.mvc.method.annotation.RequestBodyAdvice
    + org.springframework.web.servlet.mvc.method.annotation.RequestBodyAdviceAdapter
        + org.springframework.web.servlet.mvc.method.annotation.JsonViewRequestBodyAdvice
```

## ResponseBodyAdvice

```java
org.springframework.web.servlet.mvc.method.annotation.ResponseBodyAdvice<T>
    + org.springframework.web.servlet.mvc.method.annotation.AbstractMappingJacksonResponseBodyAdvice
        + org.springframework.web.servlet.mvc.method.annotation.JsonViewResponseBodyAdvice
```

## SseEventBuilder

```java
org.springframework.web.servlet.mvc.method.annotation.SseEmitter.SseEventBuilder
org.springframework.web.servlet.mvc.method.annotation.StreamingResponseBody
```

## RedirectAttributes

```java
org.springframework.web.servlet.mvc.support.RedirectAttributes
    + org.springframework.web.servlet.mvc.support.RedirectAttributesModelMap
```

## LinkParser

```java
org.springframework.web.servlet.resource.CssLinkResourceTransformer.LinkParser
    + org.springframework.web.servlet.resource.CssLinkResourceTransformer.AbstractLinkParser
```

## HttpResource

```java
org.springframework.web.servlet.resource.HttpResource
```

## ResourceResolver

```java
org.springframework.web.servlet.resource.ResourceResolver
    + org.springframework.web.servlet.resource.AbstractResourceResolver
        + org.springframework.web.servlet.resource.CachingResourceResolver
        + org.springframework.web.servlet.resource.EncodedResourceResolver
        + org.springframework.web.servlet.resource.GzipResourceResolver
        + org.springframework.web.servlet.resource.PathResourceResolver
        + org.springframework.web.servlet.resource.VersionResourceResolver
        + org.springframework.web.servlet.resource.WebJarsResourceResolver

org.springframework.web.servlet.resource.ResourceResolverChain
```

## ResourceTransformer

```java
org.springframework.web.servlet.resource.ResourceTransformer
    + org.springframework.web.servlet.resource.CachingResourceTransformer
    + org.springframework.web.servlet.resource.ResourceTransformerSupport
        + org.springframework.web.servlet.resource.AppCacheManifestTransformer
        + org.springframework.web.servlet.resource.CssLinkResourceTransformer

org.springframework.web.servlet.resource.ResourceTransformerChain
```

## VersionPathStrategy

```java
org.springframework.web.servlet.resource.VersionPathStrategy
    + org.springframework.web.servlet.resource.AbstractVersionStrategy.FileNameVersionPathStrategy
    + org.springframework.web.servlet.resource.AbstractVersionStrategy.PrefixVersionPathStrategy
    + org.springframework.web.servlet.resource.VersionStrategy
        + org.springframework.web.servlet.resource.AbstractVersionStrategy
            + org.springframework.web.servlet.resource.ContentVersionStrategy
            + org.springframework.web.servlet.resource.FixedVersionStrategy
```

## RequestDataValueProcessor

```java
org.springframework.web.servlet.support.RequestDataValueProcessor
```

## ArgumentAware

```java
org.springframework.web.servlet.tags.ArgumentAware
    + org.springframework.web.servlet.tags.MessageTag
        + org.springframework.web.servlet.tags.ThemeTag
```

## EditorAwareTag

```java
org.springframework.web.servlet.tags.EditorAwareTag
    + org.springframework.web.servlet.tags.form.AbstractDataBoundFormElementTag
        + org.springframework.web.servlet.tags.form.AbstractHtmlElementTag
            + org.springframework.web.servlet.tags.form.AbstractHtmlElementBodyTag
                + org.springframework.web.servlet.tags.form.ErrorsTag
                + org.springframework.web.servlet.tags.form.OptionTag
            + org.springframework.web.servlet.tags.form.AbstractHtmlInputElementTag
                + org.springframework.web.servlet.tags.form.AbstractCheckedElementTag
                    + org.springframework.web.servlet.tags.form.AbstractMultiCheckedElementTag
                        + org.springframework.web.servlet.tags.form.CheckboxesTag
                        + org.springframework.web.servlet.tags.form.RadioButtonsTag
                    + org.springframework.web.servlet.tags.form.AbstractSingleCheckedElementTag
                        + org.springframework.web.servlet.tags.form.CheckboxTag
                        + org.springframework.web.servlet.tags.form.RadioButtonTag
                + org.springframework.web.servlet.tags.form.InputTag
                    + org.springframework.web.servlet.tags.form.PasswordInputTag
                + org.springframework.web.servlet.tags.form.SelectTag
                + org.springframework.web.servlet.tags.form.TextareaTag
            + org.springframework.web.servlet.tags.form.ButtonTag
            + org.springframework.web.servlet.tags.form.FormTag
            + org.springframework.web.servlet.tags.form.HiddenInputTag
            + org.springframework.web.servlet.tags.form.LabelTag
            + org.springframework.web.servlet.tags.form.OptionsTag
    + org.springframework.web.servlet.tags.BindTag
```

## ParamAware

```java
org.springframework.web.servlet.tags.ParamAware
    + org.springframework.web.servlet.tags.UrlTag
```

## CacheFilter

```java
org.springframework.web.servlet.view.AbstractCachingViewResolver.CacheFilter
```

## FreeMarkerConfig

```java
org.springframework.web.servlet.view.freemarker.FreeMarkerConfig
    + org.springframework.web.servlet.view.freemarker.FreeMarkerConfigurer
```

## GroovyMarkupConfig

```java
org.springframework.web.servlet.view.groovy.GroovyMarkupConfig
    + org.springframework.web.servlet.view.groovy.GroovyMarkupConfigurer
```

## ScriptTemplateConfig

```java
org.springframework.web.servlet.view.script.ScriptTemplateConfig
    + org.springframework.web.servlet.view.script.ScriptTemplateConfigurer
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



































