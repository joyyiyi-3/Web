## padding 填充单面

具有用于指定元素每侧填充的属性：

- padding-top
- padding-right
- padding-bottom
- padding-left
  所有填充属性都可以具有以下值：

- 长度- 指定 px、pt、cm 等的填充。
- % - 指定包含元素宽度的百分比填充
- 继承 - 指定应从父元素继承填充
  ** 注意：不允许使用负值。**

## padding 简写属性

该 padding 属性是以下各个填充属性的简写属性：

- padding-top
- padding-right
- padding-bottom
- padding-left

padding 也可以有 1~4 个值，跟 margin 和 border 一样

## 关于元素宽度

此 CSSwidth 属性指定元素内容区域的宽度。内容区域是指元素的内边距 (padding)、边框 (border) 和外边距 (margin) 内的部分（标准盒模型）。因此，添加到该元素的填充将添加到元素的总宽度中（标准盒模型）

**例子 1**

这里， `<div> `元素的宽度被设置为 300px。然而， `<div>` 元素的实际宽度将是 350px（300px + 25px 左内边距 + 25px 右内边距）：

```
div {
  width: 300px;
  padding: 25px;
}
```

**例子 2**
无论填充量是多少，都可以使用该 box-sizing 属性(变成替换盒模型)来保持元素宽度为 300px。这会使元素保持其实际宽度；如果增加填充量（padding），可用的内容空间将会减少。

```
div {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
}
```
