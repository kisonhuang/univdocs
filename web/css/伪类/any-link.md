# :any-link

:any-link伪类选择器
+ 匹配作为链接源锚的元素，无论是否被访问。
+ 匹配所有具有href属性的`<a>`元素和`<area>`元素。
+ 匹配所有:link或:visited匹配的元素。

## 示例

匹配所有具有href属性的a元素

+ HTML

```
<a href="https://example.com">外部链接</a><br>
<a href="#">内部链接</a><br>
<a>占位符链接（没有设置样式）</a>
```

+ CSS

```
a:any-link {
  border: 1px solid blue;
  color: orange;
}
```

+ CSS：WebKit浏览器

```
a:-webkit-any-link {
  border: 1px solid blue;
  color: orange;
}
```

## 规范

https://developer.mozilla.org/en-US/docs/Web/CSS/:any-link#specifications

## 兼容性

https://developer.mozilla.org/en-US/docs/Web/CSS/:any-link#browser_compatibility

## 参阅

https://developer.mozilla.org/en-US/docs/Web/CSS/:any-link#see_also




