# Spring Boot依赖

## spring-boot-dependencies

```xml
<parent>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-dependencies</artifactId>
	<version>2.5.0</version>
</parent>
```

```xml
<dependencyManagement>
	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-dependencies</artifactId>
			<version>2.5.0</version>
			<type>pom</type>
			<scope>import</scope>
		</dependency>
	</dependencies>
</dependencyManagement>
```

## spring-boot-starter-parent

```xml
<parent>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-parent</artifactId>
	<version>2.5.0</version>
</parent>
```

```xml
<dependencyManagement>
	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-parent</artifactId>
			<version>2.5.0</version>
			<type>pom</type>
			<scope>import</scope>
		</dependency>
	</dependencies>
</dependencyManagement>
```

## spring-boot-maven-plugin

```xml
<build>
	<plugins>
		<plugin>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-maven-plugin</artifactId>
		</plugin>
	</plugins>
</build>
```

## spring-boot-project

```xml
spring-boot
spring-boot-autoconfigure
spring-boot-autoconfigure-processor
spring-boot-configuration-metadata
spring-boot-configuration-processor
spring-boot-test
spring-boot-test-autoconfigure
spring-boot-actuator
spring-boot-actuator-autoconfigure
spring-boot-loader
spring-boot-loader-tools
spring-boot-devtools
spring-boot-buildpack-platform
spring-boot-jarmode-layertools
spring-boot-properties-migrator
```

```xml
spring-boot-cli
spring-boot-dependencies
spring-boot-parent
spring-boot-docs
spring-boot-starters
spring-boot-tools
```

## Spring Boot启动器

```xml
<dependencies>
	<dependency>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-web</artifactId>
	</dependency>
</dependencies>
```

### Spring Boot应用程序启动器

```xml
spring-boot-starter
spring-boot-starter-activemq
spring-boot-starter-amqp
spring-boot-starter-aop
spring-boot-starter-artemis
spring-boot-starter-batch
spring-boot-starter-cache
spring-boot-starter-data-cassandra
spring-boot-starter-data-cassandra-reactive
spring-boot-starter-data-couchbase
spring-boot-starter-data-couchbase-reactive
spring-boot-starter-data-elasticsearch
spring-boot-starter-data-jdbc
spring-boot-starter-data-jpa
spring-boot-starter-data-ldap
spring-boot-starter-data-mongodb
spring-boot-starter-data-mongodb-reactive
spring-boot-starter-data-r2dbc
spring-boot-starter-data-redis
spring-boot-starter-data-redis-reactive
spring-boot-starter-data-neo4j
spring-boot-starter-data-rest
spring-boot-starter-freemarker
spring-boot-starter-groovy-templates
spring-boot-starter-hateoas
spring-boot-starter-integration
spring-boot-starter-jdbc
spring-boot-starter-jersey
spring-boot-starter-jooq
spring-boot-starter-json
spring-boot-starter-jta-atomikos
spring-boot-starter-mail
spring-boot-starter-mustache
spring-boot-starter-oauth2-client
spring-boot-starter-oauth2-resource-server
spring-boot-starter-quartz
spring-boot-starter-rsocket
spring-boot-starter-security
spring-boot-starter-test
spring-boot-starter-thymeleaf
spring-boot-starter-validation
spring-boot-starter-web
spring-boot-starter-webflux
spring-boot-starter-websocket
spring-boot-starter-web-services
```

### Spring Boot生产环境启动器

```xml
spring-boot-starter-actuator
```

### Spring Boot特定技术启动器

```xml
spring-boot-starter-log4j2
spring-boot-starter-logging
spring-boot-starter-reactor-netty
spring-boot-starter-undertow
spring-boot-starter-jetty
spring-boot-starter-tomcat
```

## Spring Boot依赖版本
































