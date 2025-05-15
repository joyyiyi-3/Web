## 边距

可以有不同方向，为 <p> 元素的四个边设置不同的边距：

```
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```

## 边距简写

该 margin 属性是以下各个边距属性的简写属性：
margin-top
margin-right
margin-bottom
margin-left

可以有不同值（1 个，2 个，3 个，4 个）

```
/*上下左右 */
p {
margin: 25px;
}
/_ 上下/左右 _/
p {
margin: 25px 50px;
}
/_ 上/左右/下 _/
p {
margin: 25px 50px 75px;
}
/_ 上 右 下 左 _/
p {
margin: 25px 50px 75px 100px;
}
```

## 边距自动值水平居中

您可以将边距属性设置为 auto 使元素在其容器内水平居中。
然后，元素将占据指定的宽度，剩余空间将在左右边距之间平均分配。

```
div {
  width: 300px;
  margin: auto;
  border: 1px solid red;
}
```

如果去掉 width,元素宽度变为父容器的 100%（默认的块级元素行为），此时 margin: auto;无法实现水平居中，因为元素已经占满父容器，左右外边距为 0。

## 继承值

此示例让 `<p class="ex1">` 元素的左边距从父元素 (`<div>`) 继承,如果 p 不是 div 的子标签就不能继承：

```

div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
<div>
<p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
</div>
```

## 边距折叠

```
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
```

在上面的例子中，<h1> 元素的下边距为 50px，而 <h2> 元素的上边距设置为 20px。

按照常识， <h1> 和 <h2> 之间的垂直边距应该为 70px（50px + 20px）。但由于边距折叠，实际边距最终为 50px。
