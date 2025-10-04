## max 函数 / min 函数

使用 max() 将 #div1 的宽度设置为最大值，50% 或 300px：

```
#div1 {
  background-color: yellow;
  height: 100px;
  width: max(50%, 300px);
}
```

## calc()函数

使用 calc() 计算 <div> 元素的宽度：

```
#div1 {
  position: absolute; /*相对视口元素，因为没有设置父级元素*/
  left: 50px;  /*容器左边缘距离视口左边界 50px*/
  width: calc(100% - 100px);
  border: 1px solid black;
  background-color: yellow;
  padding: 5px;
}
```
