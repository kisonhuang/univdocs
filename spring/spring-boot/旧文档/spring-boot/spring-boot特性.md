# Spring Boot特性

## SpringApplication

启动Spring应用程序

```java
public static void main(String[] args) {
    SpringApplication.run(MySpringConfiguration.class, args);
}
```


### 4.1.4. 定制SpringApplication

```java
public static void main(String[] args) {
    SpringApplication app = new SpringApplication(MySpringConfiguration.class);
    app.setBannerMode(Banner.Mode.OFF);
    app.run(args);
}
```




