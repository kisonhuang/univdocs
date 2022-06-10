# :active

:active伪类选择器
+ 匹配用户激活的元素，使用鼠标时，激活开始于用户按下鼠标主按钮时。
+ 通常用于`<a>`元素和`<button>`元素，以及激活元素中包含的元素，表单元素通过关联的`<label>`元素来激活。
+ 应该按照以下顺序设置链接的样式：:link、:visited、:hover、:active。
+ 在多按钮鼠标系统中，:active伪类只应用于主按钮，即右手鼠标的最左边按钮。

## 示例

匹配已激活的链接

+ HTML

```
<p>
  这个段落包含一个链接：
  <a href="#">当你点击链接时，链接会变成红色。</a>
  当你点击段落或链接时，段落的背景色会变成灰色。
</p>
```

+ CSS

```
a:link { color: blue; }          /* 未访问的链接 */
a:visited { color: purple; }     /* 已访问的链接 */
a:hover { background: yellow; }  /* 鼠标悬停链接 */
a:active { color: red; }         /* 已激活的链接 */

p:active { background: #eee; }   /* 已激活的段落 */
```

匹配已激活的表单元素

+ HTML

```
<form>
  <label for="my-button">标签：</label>
  <button id="my-button" type="button">请点击按钮或标签！</button>
</form>
```

+ CSS

```
/* 已激活的表单元素：标签或按钮 */
form :active {
  color: red;
}

form button {
  background: white;
}
```

## 规范

https://developer.mozilla.org/en-US/docs/Web/CSS/:active#specifications

## 兼容性

https://developer.mozilla.org/en-US/docs/Web/CSS/:active#browser_compatibility

## 参阅

https://developer.mozilla.org/en-US/docs/Web/CSS/:active#see_also




