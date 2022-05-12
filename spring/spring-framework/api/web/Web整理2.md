# web

## 

```java

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

## LocaleContextResolver

```java
org.springframework.web.server.i18n.LocaleContextResolver
    + org.springframework.web.server.i18n.AcceptHeaderLocaleContextResolver
    + org.springframework.web.server.i18n.FixedLocaleContextResolver
```

## ThemeResolver

```java
org.springframework.web.servlet.ThemeResolver
    + org.springframework.web.servlet.theme.AbstractThemeResolver
        + org.springframework.web.servlet.theme.FixedThemeResolver
        + org.springframework.web.servlet.theme.SessionThemeResolver
    + org.springframework.web.servlet.theme.CookieThemeResolver
```

## FlashMapManager

```java
org.springframework.web.servlet.FlashMapManager
    + org.springframework.web.servlet.support.AbstractFlashMapManager
        + org.springframework.web.servlet.support.SessionFlashMapManager
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

## 

```java

```

## 

```java

```

## 

```java

```



































