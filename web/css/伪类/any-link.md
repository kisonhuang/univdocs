# :any-link

:any-link CSS伪类选择器匹配作为链接源锚的元素，无论链接是否被访问。

:any-link CSS伪类选择器匹配所有具有href属性的a和area元素。

:any-link CSS伪类选择器匹配所有:link或:visited匹配的元素。

## 示例

设置所有具有href属性的a元素的边框和颜色

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




