# :autofill

:autofill伪类选择器
+ 匹配浏览器自动填充输入值的`<input>`元素。
+ 用户编辑`<input>`元素时停止匹配。

很多浏览器的用户代理样式表在其:-webkit-autofill样式声明中使用了!important，不求助于JavaScript黑客的话，这些样式不可被网页覆盖。

例如，Chrome浏览器的内部样式表中存在以下内容：

```
background-color: rgb(232, 240, 254) !important;
background-image: none !important;
color: -internal-light-dark(black, white) !important;
```

这意味着不能在自己的规则中设置：background-color、background-image或color。

## 示例

匹配浏览器自动填充邮件的`<input>`元素

+ HTML

```
<form method="post" action="">
  <label for="email">邮件</label>
  <input type="email" name="email" id="email" autocomplete="email">
</form>
```

+ CSS

```
input {
  border: 3px solid grey;
  border-radius: 3px;
}

input:autofill {
  border: 3px solid blue;
}

/* WebKit浏览器 */
input:-webkit-autofill {
  border: 3px solid blue;
}
```

## 规范

https://developer.mozilla.org/en-US/docs/Web/CSS/:autofill#specifications

## 兼容性

https://developer.mozilla.org/en-US/docs/Web/CSS/:autofill#browser_compatibility

## 参阅

https://developer.mozilla.org/en-US/docs/Web/CSS/:autofill#see_also




