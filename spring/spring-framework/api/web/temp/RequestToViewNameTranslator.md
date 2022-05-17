# RequestToViewNameTranslator

```java
org.springframework.web.servlet.RequestToViewNameTranslator
    + org.springframework.web.servlet.view.DefaultRequestToViewNameTranslator
```

## RequestToViewNameTranslator

```java
## 接口方法
getViewName(HttpServletRequest request)           没有提供视图名时，把HttpServletRequest转换为逻辑视图名
```

## DefaultRequestToViewNameTranslator

```java
## 接口方法
getViewName(HttpServletRequest request)           没有提供视图名时，把HttpServletRequest的URI转换为逻辑视图名

## 配置属性
String prefix              = ""                   前缀
String suffix              = ""                   后缀
String separator           = "/"                  分隔符
boolean stripLeadingSlash  = true                 是否去掉开头斜杠
boolean stripTrailingSlash = true                 是否去掉结尾斜杠
boolean stripExtension     = true                 是否去掉扩展名

## 配置方法
setPrefix(String prefix)                          设置前缀
setSuffix(String suffix)                          设置后缀
setSeparator(String separator)                    设置分隔符
setStripLeadingSlash(boolean stripLeadingSlash)   设置是否去掉开头斜杠
setStripTrailingSlash(boolean stripTrailingSlash) 设置是否去掉结尾斜杠
setStripExtension(boolean stripExtension)         设置是否去掉扩展名
```

## 示例

```
## 转换示例
http://localhost:8080/gamecast/display.html             >> display
http://localhost:8080/gamecast/displayShoppingCart.html >> displayShoppingCart
http://localhost:8080/gamecast/admin/index.html         >> admin/index
```




