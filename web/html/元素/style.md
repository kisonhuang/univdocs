# style

style元素是。

The <style> HTML element contains style information for a document, or part of a document. 

It contains CSS, which is applied to the contents of the document containing the <style> element.


The <style> element must be included inside the <head> of the document. 

In general, it is better to put your styles in external stylesheets and apply them using <link> elements.

If you include multiple <style> and <link> elements in your document, 

they will be applied to the DOM in the order they are included in the document — make sure you include them in the correct order, 

to avoid unexpected cascade issues.

In the same manner as <link> elements, <style> elements can include media attributes that contain media queries, 

allowing you to selectively apply internal stylesheets to your document depending on media features such as viewport width.









```
内容分类：
允许内容：流
允许上级：
忽略标签：可以省略开始标签；可以省略结束标签
隐式ARIA：通用
允许ARIA：无
DOM接口：
访问方式：
```

## 属性

可用属性

```
全局属性

```

废弃属性

```

```

## 示例

```
<!doctype html>
<html>
<head>
  <style>
    p {
      color: red;
    }
  </style>
</head>
<body>
  <p>This is my paragraph.</p>
</body>
</html>
```



```
<!doctype html>
<html>
<head>
  <style>
    p {
      color: white;
      background-color: blue;
      padding: 5px;
      border: 1px solid black;
    }
  </style>
  <style>
    p {
      color: blue;
      background-color: yellow;
    }
  </style>
</head>
<body>
  <p>This is my paragraph.</p>
</body>
</html>
```


```
<!doctype html>
<html>
<head>
  <style>
    p {
      color: white;
      background-color: blue;
      padding: 5px;
      border: 1px solid black;
    }
  </style>
  <style media="all and (max-width: 500px)">
    p {
      color: blue;
      background-color: yellow;
    }
  </style>
</head>
<body>
  <p>This is my paragraph.</p>
</body>
</html>
```








## 规范



## 兼容性



## 参阅






