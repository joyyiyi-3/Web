## 什么是伪元素？

CSS 伪元素可以用来设置元素特定部分的样式
如：

- 设置元素首字母或首行的样式
- 在元素之前或之后插入内容
- 设置列表项标记的样式
- 设置对话框后面的视图框的样式

## ::first-line 伪元素

伪元素::first-line 用于给文本的第一行添加特殊样式。

```
p::first-line {
  color: #ff0000;
  font-variant: small-caps;
}
```

注意：伪::first-line 元素只能应用于块级元素。

下列属性适用于::first-line 伪元素：

字体属性
颜色属性
背景属性
字间距
字母间距
文字装饰
垂直对齐
文本转换
行高
清除

## ::first-letter 伪元素

伪元素::first-letter 用于给文本的首字母添加特殊样式。

```
p::first-letter {
  color: #ff0000;
  font-size: xx-large;
}
```

注意：伪::first-letter 元素只能应用于块级元素。适用属性和上面一样

## 伪元素和 HTML 类结合

```
p.intro::first-letter {
  color: #ff0000;
  font-size: 200%;
}
```

## ::before 伪元素

伪元素::before 可用于在元素内容之前插入一些内容。

以下示例在每个 <h1> 元素的内容之前插入一张图片：

```
h1::before {
  content: url(smiley.gif);
}
```

::after 同理

## ::marker 伪元素

伪元素::marker 选择列表项的标记。
以下示例设置列表项的标记样式：

```
::marker {
  color: red;
  font-size: 23px;
}
```

## ::selection 伪元素

伪元素::selection 与用户选择的元素部分匹配。

以下 CSS 属性可应用于::selection：
color，background，cursor，outline

下面的示例使所选文本在黄色背景上显示为红色：
![alt text](::selection 伪元素使用.png)
