## 后代组合器 --- (空格)

下面选中所有 div 元素内部的 p 元素，包括那些被其他元素嵌套的 p 元素

```
div p {
  background-color: yellow;
}
```

## 子组合器 --- (>)

下面选中所有 div 元素内部的直接 p 元素，但是不包括那些被其他元素嵌套的 p 元素

```
div > p {
  background-color: yellow;
}
```

## 下一个兄弟组合器 (+)

下面选中紧挨着 div 元素的下一个同级 p 元素（仅一个）

```
div + p {
  background-color: yellow;
}
```

## 后续兄弟组合器（~）

下面选中 div 元素后**所有**同级 p 元素

```
div ~ p {
  background-color: yellow;
}
```
