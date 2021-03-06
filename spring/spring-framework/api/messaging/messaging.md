# messaging

```java
org.springframework.messaging.Message
org.springframework.messaging.MessageChannel
org.springframework.messaging.MessageDeliveryException
org.springframework.messaging.MessageHandler
org.springframework.messaging.MessageHandlingException
org.springframework.messaging.MessageHeaders
org.springframework.messaging.MessagingException
org.springframework.messaging.PollableChannel
org.springframework.messaging.ReactiveMessageHandler
org.springframework.messaging.SubscribableChannel

org.springframework.messaging.converter.AbstractJsonMessageConverter
org.springframework.messaging.converter.AbstractMessageConverter
org.springframework.messaging.converter.ByteArrayMessageConverter
org.springframework.messaging.converter.CompositeMessageConverter
org.springframework.messaging.converter.ContentTypeResolver
org.springframework.messaging.converter.DefaultContentTypeResolver
org.springframework.messaging.converter.GenericMessageConverter
org.springframework.messaging.converter.GsonMessageConverter
org.springframework.messaging.converter.JsonbMessageConverter
org.springframework.messaging.converter.KotlinSerializationJsonMessageConverter
org.springframework.messaging.converter.MappingJackson2MessageConverter
org.springframework.messaging.converter.MarshallingMessageConverter
org.springframework.messaging.converter.MessageConversionException
org.springframework.messaging.converter.MessageConverter
org.springframework.messaging.converter.ProtobufJsonFormatMessageConverter
org.springframework.messaging.converter.ProtobufMessageConverter
org.springframework.messaging.converter.SimpleMessageConverter
org.springframework.messaging.converter.SmartMessageConverter
org.springframework.messaging.converter.StringMessageConverter

org.springframework.messaging.core.AbstractDestinationResolvingMessagingTemplate
org.springframework.messaging.core.AbstractMessageReceivingTemplate
org.springframework.messaging.core.AbstractMessageSendingTemplate
org.springframework.messaging.core.AbstractMessagingTemplate
org.springframework.messaging.core.BeanFactoryMessageChannelDestinationResolver
org.springframework.messaging.core.CachingDestinationResolverProxy
org.springframework.messaging.core.DestinationResolutionException
org.springframework.messaging.core.DestinationResolver
org.springframework.messaging.core.DestinationResolvingMessageReceivingOperations
org.springframework.messaging.core.DestinationResolvingMessageRequestReplyOperations
org.springframework.messaging.core.DestinationResolvingMessageSendingOperations
org.springframework.messaging.core.GenericMessagingTemplate
org.springframework.messaging.core.MessagePostProcessor
org.springframework.messaging.core.MessageReceivingOperations
org.springframework.messaging.core.MessageRequestReplyOperations
org.springframework.messaging.core.MessageSendingOperations

org.springframework.messaging.handler.AbstractMessageCondition
org.springframework.messaging.handler.annotation.DestinationVariable
org.springframework.messaging.handler.annotation.Header
org.springframework.messaging.handler.annotation.Headers
org.springframework.messaging.handler.annotation.MessageExceptionHandler
org.springframework.messaging.handler.annotation.MessageMapping
org.springframework.messaging.handler.annotation.Payload
org.springframework.messaging.handler.annotation.reactive.AbstractNamedValueMethodArgumentResolver
org.springframework.messaging.handler.annotation.reactive.AbstractNamedValueMethodArgumentResolver.NamedValueInfo
org.springframework.messaging.handler.annotation.reactive.ContinuationHandlerMethodArgumentResolver
org.springframework.messaging.handler.annotation.reactive.DestinationVariableMethodArgumentResolver
org.springframework.messaging.handler.annotation.reactive.HeaderMethodArgumentResolver
org.springframework.messaging.handler.annotation.reactive.HeadersMethodArgumentResolver
org.springframework.messaging.handler.annotation.reactive.MessageMappingMessageHandler
org.springframework.messaging.handler.annotation.reactive.PayloadMethodArgumentResolver
org.springframework.messaging.handler.annotation.SendTo
org.springframework.messaging.handler.annotation.support.AbstractNamedValueMethodArgumentResolver
org.springframework.messaging.handler.annotation.support.AbstractNamedValueMethodArgumentResolver.NamedValueInfo
org.springframework.messaging.handler.annotation.support.AnnotationExceptionHandlerMethodResolver
org.springframework.messaging.handler.annotation.support.DefaultMessageHandlerMethodFactory
org.springframework.messaging.handler.annotation.support.DestinationVariableMethodArgumentResolver
org.springframework.messaging.handler.annotation.support.HeaderMethodArgumentResolver
org.springframework.messaging.handler.annotation.support.HeadersMethodArgumentResolver
org.springframework.messaging.handler.annotation.support.MessageHandlerMethodFactory
org.springframework.messaging.handler.annotation.support.MessageMethodArgumentResolver
org.springframework.messaging.handler.annotation.support.MethodArgumentNotValidException
org.springframework.messaging.handler.annotation.support.MethodArgumentTypeMismatchException
org.springframework.messaging.handler.annotation.support.PayloadArgumentResolver
org.springframework.messaging.handler.annotation.support.PayloadMethodArgumentResolver
org.springframework.messaging.handler.annotation.ValueConstants
org.springframework.messaging.handler.CompositeMessageCondition
org.springframework.messaging.handler.DestinationPatternsMessageCondition
org.springframework.messaging.handler.HandlerMethod
org.springframework.messaging.handler.invocation.AbstractAsyncReturnValueHandler
org.springframework.messaging.handler.invocation.AbstractExceptionHandlerMethodResolver
org.springframework.messaging.handler.invocation.AbstractMethodMessageHandler
org.springframework.messaging.handler.invocation.AsyncHandlerMethodReturnValueHandler
org.springframework.messaging.handler.invocation.CompletableFutureReturnValueHandler
org.springframework.messaging.handler.invocation.HandlerMethodArgumentResolver
org.springframework.messaging.handler.invocation.HandlerMethodArgumentResolverComposite
org.springframework.messaging.handler.invocation.HandlerMethodReturnValueHandler
org.springframework.messaging.handler.invocation.HandlerMethodReturnValueHandlerComposite
org.springframework.messaging.handler.invocation.InvocableHandlerMethod
org.springframework.messaging.handler.invocation.ListenableFutureReturnValueHandler
org.springframework.messaging.handler.invocation.MethodArgumentResolutionException
org.springframework.messaging.handler.invocation.reactive.AbstractEncoderMethodReturnValueHandler
org.springframework.messaging.handler.invocation.reactive.AbstractMethodMessageHandler
org.springframework.messaging.handler.invocation.reactive.ArgumentResolverConfigurer
org.springframework.messaging.handler.invocation.reactive.HandlerMethodArgumentResolver
org.springframework.messaging.handler.invocation.reactive.HandlerMethodArgumentResolverComposite
org.springframework.messaging.handler.invocation.reactive.HandlerMethodReturnValueHandler
org.springframework.messaging.handler.invocation.reactive.HandlerMethodReturnValueHandlerComposite
org.springframework.messaging.handler.invocation.reactive.InvocableHandlerMethod
org.springframework.messaging.handler.invocation.reactive.ReturnValueHandlerConfigurer
org.springframework.messaging.handler.invocation.reactive.SyncHandlerMethodArgumentResolver
org.springframework.messaging.handler.invocation.ReactiveReturnValueHandler
org.springframework.messaging.handler.MessageCondition
org.springframework.messaging.handler.MessagingAdviceBean

org.springframework.messaging.rsocket.annotation.ConnectMapping
org.springframework.messaging.rsocket.annotation.support.RSocketFrameTypeMessageCondition
org.springframework.messaging.rsocket.annotation.support.RSocketMessageHandler
org.springframework.messaging.rsocket.annotation.support.RSocketPayloadReturnValueHandler
org.springframework.messaging.rsocket.annotation.support.RSocketRequesterMethodArgumentResolver
org.springframework.messaging.rsocket.DefaultMetadataExtractor
org.springframework.messaging.rsocket.MetadataExtractor
org.springframework.messaging.rsocket.MetadataExtractorRegistry
org.springframework.messaging.rsocket.PayloadUtils
org.springframework.messaging.rsocket.RSocketConnectorConfigurer
org.springframework.messaging.rsocket.RSocketRequester
org.springframework.messaging.rsocket.RSocketRequester.Builder
org.springframework.messaging.rsocket.RSocketRequester.MetadataSpec
org.springframework.messaging.rsocket.RSocketRequester.RequestSpec
org.springframework.messaging.rsocket.RSocketRequester.RetrieveSpec
org.springframework.messaging.rsocket.RSocketStrategies
org.springframework.messaging.rsocket.RSocketStrategies.Builder

org.springframework.messaging.simp.annotation.SendToUser
org.springframework.messaging.simp.annotation.SubscribeMapping
org.springframework.messaging.simp.annotation.support.MissingSessionUserException
org.springframework.messaging.simp.annotation.support.PrincipalMethodArgumentResolver
org.springframework.messaging.simp.annotation.support.SendToMethodReturnValueHandler
org.springframework.messaging.simp.annotation.support.SimpAnnotationMethodMessageHandler
org.springframework.messaging.simp.annotation.support.SubscriptionMethodReturnValueHandler
org.springframework.messaging.simp.broker.AbstractBrokerMessageHandler
org.springframework.messaging.simp.broker.AbstractSubscriptionRegistry
org.springframework.messaging.simp.broker.BrokerAvailabilityEvent
org.springframework.messaging.simp.broker.DefaultSubscriptionRegistry
org.springframework.messaging.simp.broker.OrderedMessageChannelDecorator
org.springframework.messaging.simp.broker.SimpleBrokerMessageHandler
org.springframework.messaging.simp.broker.SubscriptionRegistry
org.springframework.messaging.simp.config.AbstractBrokerRegistration
org.springframework.messaging.simp.config.AbstractMessageBrokerConfiguration
org.springframework.messaging.simp.config.ChannelRegistration
org.springframework.messaging.simp.config.MessageBrokerRegistry
org.springframework.messaging.simp.config.SimpleBrokerRegistration
org.springframework.messaging.simp.config.StompBrokerRelayRegistration
org.springframework.messaging.simp.config.TaskExecutorRegistration
org.springframework.messaging.simp.SimpAttributes
org.springframework.messaging.simp.SimpAttributesContextHolder
org.springframework.messaging.simp.SimpLogging
org.springframework.messaging.simp.SimpMessageHeaderAccessor
org.springframework.messaging.simp.SimpMessageMappingInfo
org.springframework.messaging.simp.SimpMessageSendingOperations
org.springframework.messaging.simp.SimpMessageType
org.springframework.messaging.simp.SimpMessageTypeMessageCondition
org.springframework.messaging.simp.SimpMessagingTemplate
org.springframework.messaging.simp.SimpSessionScope
org.springframework.messaging.simp.stomp.BufferingStompDecoder
org.springframework.messaging.simp.stomp.ConnectionHandlingStompSession
org.springframework.messaging.simp.stomp.ConnectionLostException
org.springframework.messaging.simp.stomp.DefaultStompSession
org.springframework.messaging.simp.stomp.ReactorNettyTcpStompClient
org.springframework.messaging.simp.stomp.StompBrokerRelayMessageHandler
org.springframework.messaging.simp.stomp.StompBrokerRelayMessageHandler.Stats
org.springframework.messaging.simp.stomp.StompClientSupport
org.springframework.messaging.simp.stomp.StompCommand
org.springframework.messaging.simp.stomp.StompConversionException
org.springframework.messaging.simp.stomp.StompDecoder
org.springframework.messaging.simp.stomp.StompEncoder
org.springframework.messaging.simp.stomp.StompFrameHandler
org.springframework.messaging.simp.stomp.StompHeaderAccessor
org.springframework.messaging.simp.stomp.StompHeaders
org.springframework.messaging.simp.stomp.StompReactorNettyCodec
org.springframework.messaging.simp.stomp.StompSession
org.springframework.messaging.simp.stomp.StompSession.Receiptable
org.springframework.messaging.simp.stomp.StompSession.Subscription
org.springframework.messaging.simp.stomp.StompSessionHandler
org.springframework.messaging.simp.stomp.StompSessionHandlerAdapter
org.springframework.messaging.simp.stomp.StompTcpConnectionHandler
org.springframework.messaging.simp.user.DefaultUserDestinationResolver
org.springframework.messaging.simp.user.DestinationUserNameProvider
org.springframework.messaging.simp.user.MultiServerUserRegistry
org.springframework.messaging.simp.user.SimpSession
org.springframework.messaging.simp.user.SimpSubscription
org.springframework.messaging.simp.user.SimpSubscriptionMatcher
org.springframework.messaging.simp.user.SimpUser
org.springframework.messaging.simp.user.SimpUserRegistry
org.springframework.messaging.simp.user.UserDestinationMessageHandler
org.springframework.messaging.simp.user.UserDestinationResolver
org.springframework.messaging.simp.user.UserDestinationResult
org.springframework.messaging.simp.user.UserRegistryMessageHandler

org.springframework.messaging.support.AbstractHeaderMapper
org.springframework.messaging.support.AbstractMessageChannel
org.springframework.messaging.support.AbstractSubscribableChannel
org.springframework.messaging.support.ChannelInterceptor
org.springframework.messaging.support.ChannelInterceptorAdapter
org.springframework.messaging.support.ErrorMessage
org.springframework.messaging.support.ExecutorChannelInterceptor
org.springframework.messaging.support.ExecutorSubscribableChannel
org.springframework.messaging.support.GenericMessage
org.springframework.messaging.support.HeaderMapper
org.springframework.messaging.support.IdTimestampMessageHeaderInitializer
org.springframework.messaging.support.ImmutableMessageChannelInterceptor
org.springframework.messaging.support.InterceptableChannel
org.springframework.messaging.support.MessageBuilder
org.springframework.messaging.support.MessageHandlingRunnable
org.springframework.messaging.support.MessageHeaderAccessor
org.springframework.messaging.support.MessageHeaderInitializer
org.springframework.messaging.support.NativeMessageHeaderAccessor

org.springframework.messaging.tcp.FixedIntervalReconnectStrategy
org.springframework.messaging.tcp.reactor.AbstractNioBufferReactorNettyCodec
org.springframework.messaging.tcp.reactor.ReactorNettyCodec
org.springframework.messaging.tcp.reactor.ReactorNettyTcpClient
org.springframework.messaging.tcp.reactor.ReactorNettyTcpConnection
org.springframework.messaging.tcp.ReconnectStrategy
org.springframework.messaging.tcp.TcpConnection
org.springframework.messaging.tcp.TcpConnectionHandler
org.springframework.messaging.tcp.TcpOperations
```















