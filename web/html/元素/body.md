# html

body元素是HTML文档的内容，一个文档只能有一个body元素。

```
内容分类：节的根元素
允许内容：流
允许上级：html元素的第二个子元素
忽略标签：body元素中第一项不是空格、注释、script元素或style元素时，可以省略开始标签；body元素有内容或开始标签，并且body元素后没有紧跟着注释时，可以省略结束标签
隐式ARIA：通用
允许ARIA：无
DOM接口：HTMLBodyElement
访问方式：document.body
```

## 属性

可用属性

```
全局属性
onload           Function to call when the document has finished loading.
onbeforeunload   Function to call when the document is about to be unloaded.
onunload         Function to call when the document is going away.
ononline         Function to call when network communication has been restored.
onoffline        Function to call when network communication has failed.
onredo           Function to call when the user has moved forward in undo transaction history.
onundo           Function to call when the user has moved backward in undo transaction history.
onbeforeprint    Function to call when the user requests printing of the document.
onafterprint     Function to call after the user has printed the document.
onfocus          Function to call when the document receives focus.
onblur           Function to call when the document loses focus.
onhashchange     Function to call when the fragment identifier part (starting with the hash ('#') character) of the document's current address has changed.
onlanguagechange Function to call when the preferred languages changed.
onstorage        Function to call when the storage area has changed.
onresize         Function to call when the document has been resized.
onpopstate       Function to call when the user has navigated session history.
onmessage        Function to call when the document has received a message.
onerror          Function to call when the document fails to load properly.
```

废弃属性

```
link             Color of text for unvisited hypertext links. 不要使用这个属性， Use the CSS color property in conjunction with the :link pseudo-class instead.
alink            Color of text for hyperlinks when selected. 不要使用这个属性， Use the CSS color property in conjunction with the :active pseudo-class instead.
vlink            Color of text for visited hypertext links. 不要使用这个属性， Use the CSS color property in conjunction with the :visited pseudo-class instead.
text             Foreground color of text. 不要使用这个属性， Use CSS color property on the element instead.
background       URI of a image to use as a background. 不要使用这个属性， Use the CSS background property on the element instead.
bgcolor          Background color for the document. 不要使用这个属性， Use the CSS background-color property on the element instead.
topmargin        The margin of the top of the body. 不要使用这个属性， Use the CSS margin-top property on the element instead.
bottommargin     The margin of the bottom of the body. 不要使用这个属性， Use the CSS margin-bottom property on the element instead.
leftmargin       The margin of the left of the body. 不要使用这个属性， Use the CSS margin-left property on the element instead.
rightmargin      The margin of the right of the body. 不要使用这个属性， Use the CSS margin-right property on the element instead.
```

## 示例

```
<html>
  <head>
    <title>Document title</title>
  </head>
  <body>
    <p>This is a paragraph</p>
  </body>
</html>
```

## 规范

https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body#specifications

## 兼容性

https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body#browser_compatibility

## 参阅

https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body#see_also




