# http

## HttpMessage

```java
org.springframework.http.HttpMessage
    + org.springframework.http.HttpInputMessage
        + org.springframework.http.converter.json.MappingJacksonInputMessage
        + org.springframework.mock.http.MockHttpInputMessage
            + org.springframework.mock.http.client.MockClientHttpResponse
        + org.springframework.http.client.ClientHttpResponse
            + org.springframework.http.client.AbstractClientHttpResponse
            + org.springframework.mock.http.client.MockClientHttpResponse
        + org.springframework.http.server.ServerHttpRequest
            + org.springframework.http.server.ServletServerHttpRequest
                + org.springframework.web.multipart.support.RequestPartServletServerHttpRequest
    + org.springframework.http.HttpOutputMessage
        + org.springframework.mock.http.MockHttpOutputMessage
            + org.springframework.mock.http.client.MockClientHttpRequest
                + org.springframework.mock.http.client.MockAsyncClientHttpRequest
        + org.springframework.http.client.AsyncClientHttpRequest
            + org.springframework.mock.http.client.MockAsyncClientHttpRequest
        + org.springframework.http.client.ClientHttpRequest
            + org.springframework.http.client.AbstractClientHttpRequest
            + org.springframework.mock.http.client.MockClientHttpRequest
                + org.springframework.mock.http.client.MockAsyncClientHttpRequest
        + org.springframework.http.server.ServerHttpResponse
            + org.springframework.http.server.DelegatingServerHttpResponse
            + org.springframework.http.server.ServletServerHttpResponse
        + org.springframework.http.StreamingHttpOutputMessage
    + org.springframework.http.HttpRequest
        + org.springframework.http.client.support.HttpRequestWrapper
        + org.springframework.http.client.AsyncClientHttpRequest
            + org.springframework.mock.http.client.MockAsyncClientHttpRequest
        + org.springframework.http.client.ClientHttpRequest
            + org.springframework.http.client.AbstractClientHttpRequest
            + org.springframework.mock.http.client.MockClientHttpRequest
                + org.springframework.mock.http.client.MockAsyncClientHttpRequest
        + org.springframework.http.server.reactive.ServerHttpRequest
            + org.springframework.http.server.reactive.AbstractServerHttpRequest
                + org.springframework.mock.http.server.reactive.MockServerHttpRequest
            + org.springframework.http.server.reactive.ServerHttpRequestDecorator
        + org.springframework.http.server.ServerHttpRequest
            + org.springframework.http.server.ServletServerHttpRequest
                + org.springframework.web.multipart.support.RequestPartServletServerHttpRequest
    + org.springframework.http.ReactiveHttpInputMessage
        + org.springframework.http.client.reactive.ClientHttpResponse
            + org.springframework.http.client.reactive.ClientHttpResponseDecorator
            + org.springframework.mock.http.client.reactive.MockClientHttpResponse
            + org.springframework.test.web.reactive.server.MockServerClientHttpResponse
        + org.springframework.http.server.reactive.ServerHttpRequest
            + org.springframework.http.server.reactive.AbstractServerHttpRequest
                + org.springframework.mock.http.server.reactive.MockServerHttpRequest
            + org.springframework.http.server.reactive.ServerHttpRequestDecorator
    + org.springframework.http.ReactiveHttpOutputMessage
        + org.springframework.http.client.reactive.ClientHttpRequest
            + org.springframework.http.client.reactive.AbstractClientHttpRequest
                + org.springframework.mock.http.client.reactive.MockClientHttpRequest
            + org.springframework.http.client.reactive.ClientHttpRequestDecorator
        + org.springframework.http.server.reactive.ServerHttpResponse
            + org.springframework.http.server.reactive.AbstractServerHttpResponse
                + org.springframework.http.server.reactive.AbstractListenerServerHttpResponse
                + org.springframework.mock.http.server.reactive.MockServerHttpResponse
            + org.springframework.http.server.reactive.ServerHttpResponseDecorator
                + org.springframework.http.server.reactive.HttpHeadResponseDecorator
        + org.springframework.http.ZeroCopyHttpOutputMessage

org.springframework.http.StreamingHttpOutputMessage.Body
org.springframework.http.server.reactive.ServerHttpRequest.Builder
```

## HttpMessageReader

```java
org.springframework.http.codec.HttpMessageReader<T>
    + org.springframework.http.codec.DecoderHttpMessageReader<T>
        + org.springframework.http.codec.ResourceHttpMessageReader
    + org.springframework.http.codec.multipart.DefaultPartHttpMessageReader
    + org.springframework.http.codec.FormHttpMessageReader
    + org.springframework.http.codec.multipart.MultipartHttpMessageReader
    + org.springframework.http.codec.ServerSentEventHttpMessageReader
    + org.springframework.http.codec.multipart.SynchronossPartHttpMessageReader
```

## HttpMessageWriter

```java
org.springframework.http.codec.HttpMessageWriter<T>
    + org.springframework.http.codec.EncoderHttpMessageWriter<T>
        + org.springframework.http.codec.protobuf.ProtobufHttpMessageWriter
    + org.springframework.http.codec.FormHttpMessageWriter
    + org.springframework.http.codec.multipart.MultipartHttpMessageWriter
    + org.springframework.http.codec.multipart.PartHttpMessageWriter
    + org.springframework.http.codec.ResourceHttpMessageWriter
    + org.springframework.http.codec.ServerSentEventHttpMessageWriter
```

## LoggingCodecSupport

```java
org.springframework.http.codec.LoggingCodecSupport
    + org.springframework.http.codec.multipart.DefaultPartHttpMessageReader
    + org.springframework.http.codec.FormHttpMessageReader
    + org.springframework.http.codec.FormHttpMessageWriter
    + org.springframework.http.codec.multipart.MultipartHttpMessageReader
    + org.springframework.http.codec.multipart.MultipartWriterSupport
        + org.springframework.http.codec.multipart.MultipartHttpMessageWriter
        + org.springframework.http.codec.multipart.PartHttpMessageWriter
    + org.springframework.http.codec.multipart.SynchronossPartHttpMessageReader
```


## Jackson2CodecSupport

```java
org.springframework.http.codec.json.Jackson2CodecSupport
    + org.springframework.http.codec.json.AbstractJackson2Decoder
        + org.springframework.http.codec.cbor.Jackson2CborDecoder
        + org.springframework.http.codec.json.Jackson2JsonDecoder
        + org.springframework.http.codec.json.Jackson2SmileDecoder
    + org.springframework.http.codec.json.AbstractJackson2Encoder
        + org.springframework.http.codec.cbor.Jackson2CborEncoder
        + org.springframework.http.codec.json.Jackson2JsonEncoder
        + org.springframework.http.codec.json.Jackson2SmileEncoder

org.springframework.http.codec.protobuf.ProtobufCodecSupport
    + org.springframework.http.codec.protobuf.ProtobufDecoder
    + org.springframework.http.codec.protobuf.ProtobufEncoder

org.springframework.http.codec.HttpMessageEncoder<T>
    + org.springframework.http.codec.json.AbstractJackson2Encoder
        + org.springframework.http.codec.cbor.Jackson2CborEncoder
        + org.springframework.http.codec.json.Jackson2JsonEncoder
        + org.springframework.http.codec.json.Jackson2SmileEncoder
    + org.springframework.http.codec.protobuf.ProtobufEncoder

org.springframework.http.codec.HttpMessageDecoder<T>
    + org.springframework.http.codec.json.AbstractJackson2Decoder
        + org.springframework.http.codec.cbor.Jackson2CborDecoder
        + org.springframework.http.codec.json.Jackson2JsonDecoder
        + org.springframework.http.codec.json.Jackson2SmileDecoder

org.springframework.http.codec.json.KotlinSerializationJsonEncoder
org.springframework.http.codec.json.KotlinSerializationJsonDecoder
org.springframework.http.codec.xml.Jaxb2XmlEncoder
org.springframework.http.codec.xml.Jaxb2XmlDecoder
org.springframework.http.codec.xml.XmlEventDecoder
```


## CodecConfigurer

```java
org.springframework.http.codec.CodecConfigurer
    + org.springframework.http.codec.ClientCodecConfigurer
        + org.springframework.http.codec.support.DefaultClientCodecConfigurer
    + org.springframework.http.codec.ServerCodecConfigurer
        + org.springframework.http.codec.support.DefaultServerCodecConfigurer
```

## PathContainer

```java

```

## HttpCookie

```java
org.springframework.http.HttpCookie
    + org.springframework.http.ResponseCookie

org.springframework.http.ResponseCookie.ResponseCookieBuilder
```

## HttpEntity

```java
org.springframework.http.HttpEntity<T>
    + org.springframework.http.RequestEntity<T>
        + org.springframework.http.RequestEntity.UriTemplateRequestEntity<T>
    + org.springframework.http.ResponseEntity<T>

org.springframework.http.ResponseEntity.HeadersBuilder<B>
    + org.springframework.http.ResponseEntity.BodyBuilder

org.springframework.http.RequestEntity.HeadersBuilder<B>
    + org.springframework.http.RequestEntity.BodyBuilder
```

## Part

```java
org.springframework.http.codec.multipart.Part
    + org.springframework.http.codec.multipart.FilePart
    + org.springframework.http.codec.multipart.FormFieldPart
```

## ClientHttpRequestFactory

```java
org.springframework.http.client.ClientHttpRequestFactory
    + org.springframework.http.client.AbstractClientHttpRequestFactoryWrapper
        + org.springframework.http.client.BufferingClientHttpRequestFactory
        + org.springframework.http.client.InterceptingClientHttpRequestFactory
    + org.springframework.http.client.HttpComponentsClientHttpRequestFactory
        + org.springframework.http.client.HttpComponentsAsyncClientHttpRequestFactory
    + org.springframework.test.web.client.MockMvcClientHttpRequestFactory
    + org.springframework.http.client.Netty4ClientHttpRequestFactory
    + org.springframework.http.client.OkHttp3ClientHttpRequestFactory
    + org.springframework.http.client.SimpleClientHttpRequestFactory

org.springframework.http.client.AsyncClientHttpRequestFactory
    + org.springframework.http.client.HttpComponentsAsyncClientHttpRequestFactory
    + org.springframework.http.client.InterceptingAsyncClientHttpRequestFactory
    + org.springframework.http.client.Netty4ClientHttpRequestFactory
    + org.springframework.http.client.OkHttp3ClientHttpRequestFactory
    + org.springframework.http.client.SimpleClientHttpRequestFactory
```

## HttpMessageConversionException

```java
org.springframework.http.converter.HttpMessageConversionException
    + org.springframework.http.converter.HttpMessageNotReadableException
    + org.springframework.http.converter.HttpMessageNotWritableException

org.springframework.http.InvalidMediaTypeException
```

## RestTemplate

```java
org.springframework.web.client.RestOperations
    + org.springframework.web.client.RestTemplate

org.springframework.web.client.AsyncRestOperations
    + org.springframework.web.client.AsyncRestTemplate

org.springframework.http.client.support.HttpAccessor
    + org.springframework.http.client.support.InterceptingHttpAccessor
        + org.springframework.web.client.RestTemplate
```

## FactoryBean

```java
org.springframework.http.client.support.ProxyFactoryBean
org.springframework.http.converter.json.GsonFactoryBean
org.springframework.http.converter.json.Jackson2ObjectMapperFactoryBean
```

## ClientHttpConnector

```java
org.springframework.http.client.reactive.ClientHttpConnector
    + org.springframework.http.client.reactive.HttpComponentsClientHttpConnector
    + org.springframework.test.web.reactive.server.HttpHandlerConnector
    + org.springframework.http.client.reactive.JettyClientHttpConnector
    + org.springframework.test.web.servlet.client.MockMvcHttpConnector
    + org.springframework.http.client.reactive.ReactorClientHttpConnector
```

## ClientHttpRequestInterceptor

```java
org.springframework.http.client.ClientHttpRequestInterceptor
    + org.springframework.http.client.support.BasicAuthenticationInterceptor
    + org.springframework.http.client.support.BasicAuthorizationInterceptor

org.springframework.http.client.AsyncClientHttpRequestInterceptor
```

## DefaultCodecs

```java
org.springframework.http.codec.CodecConfigurer.DefaultCodecs
    + org.springframework.http.codec.ClientCodecConfigurer.ClientDefaultCodecs
    + org.springframework.http.codec.ServerCodecConfigurer.ServerDefaultCodecs

org.springframework.http.codec.ClientCodecConfigurer.MultipartCodecs
org.springframework.http.codec.CodecConfigurer.CustomCodecs
org.springframework.http.codec.CodecConfigurer.DefaultCodecConfig
```

## HttpHandler

```java
org.springframework.web.server.WebHandler
    + org.springframework.web.reactive.DispatcherHandler
    + org.springframework.web.reactive.resource.ResourceWebHandler
    + org.springframework.web.server.handler.WebHandlerDecorator
        + org.springframework.web.server.handler.ExceptionHandlingWebHandler
        + org.springframework.web.server.handler.FilteringWebHandler
        + org.springframework.web.server.adapter.HttpWebHandlerAdapter

org.springframework.http.server.reactive.HttpHandler
    + org.springframework.http.server.reactive.ContextPathCompositeHandler
    + org.springframework.web.server.adapter.HttpWebHandlerAdapter

org.springframework.http.server.reactive.ServletHttpHandlerAdapter
    + org.springframework.http.server.reactive.JettyHttpHandlerAdapter
    + org.springframework.http.server.reactive.TomcatHttpHandlerAdapter

org.springframework.http.server.reactive.ReactorHttpHandlerAdapter
org.springframework.http.server.reactive.UndertowHttpHandlerAdapter
```

## ServerHttpAsyncRequestControl

```java
org.springframework.http.server.ServerHttpAsyncRequestControl
    + org.springframework.http.server.ServletServerHttpAsyncRequestControl
```

## AsyncHttpAccessor

```java
org.springframework.http.client.support.AsyncHttpAccessor
    + org.springframework.http.client.support.InterceptingAsyncHttpAccessor
    + org.springframework.web.client.AsyncRestTemplate
```

## ??????

```java
org.springframework.http.HttpHeaders
org.springframework.http.HttpMethod
org.springframework.http.HttpStatus
org.springframework.http.HttpStatus.Series

org.springframework.http.HttpRange
org.springframework.http.HttpLogging
org.springframework.http.CacheControl
org.springframework.http.ContentDisposition
org.springframework.http.ContentDisposition.Builder



org.springframework.http.codec.ServerSentEvent
org.springframework.http.codec.ServerSentEvent.Builder

org.springframework.http.converter.json.GsonBuilderUtils
org.springframework.http.converter.json.MappingJacksonValue
org.springframework.http.converter.json.Jackson2ObjectMapperBuilder
org.springframework.http.converter.json.SpringHandlerInstantiator
org.springframework.http.converter.protobuf.ExtensionRegistryInitializer

org.springframework.http.client.ClientHttpRequestInitializer
org.springframework.http.client.ClientHttpRequestExecution
org.springframework.http.client.AsyncClientHttpRequestExecution
org.springframework.http.client.MultipartBodyBuilder
org.springframework.http.client.MultipartBodyBuilder.PartBuilder

org.springframework.http.client.reactive.JettyResourceFactory
org.springframework.http.client.reactive.ReactorResourceFactory
org.springframework.http.server.reactive.AbstractListenerReadPublisher
org.springframework.http.server.reactive.AbstractListenerWriteProcessor
org.springframework.http.server.reactive.AbstractListenerWriteFlushProcessor
org.springframework.http.server.reactive.SslInfo
org.springframework.http.server.reactive.ChannelSendOperator
org.springframework.http.server.reactive.HttpHandlerDecoratorFactory
```




