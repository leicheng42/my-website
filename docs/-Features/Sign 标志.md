(sign)=
# 标志牌 Sign

符号功能允许您显示一行文本。但与 [Richtext](https://wiki.cryptovoxels.com/features/richtext) 不同，它们可以用作超链接。
![sign-example.png](https://wiki.cryptovoxels.com/sign-example.png)

## Editor

![sign-editor.png](https://wiki.cryptovoxels.com/sign-editor.png)

### Text 文本

您想要显示的文本。

### Font Size 字体大小

字体大小

### Blend mode 混合模式

这用于确定文本如何与其后面的内容混合。可用选项有 `Combine 组合` 、`Multiply 乘法` 和 `Screen 屏幕` 。

### Inverted 反转

当勾选时，文本将以白色显示在黑色背景上，而不是相反。

### Hyperlink 超链接

点击后会弹出警告消息，然后才能让玩家转到所需的链接。

### Color 颜色

字体颜色

### Background 背景

背景颜色

## 脚本属性

::::{tab-set}
:::{tab-item} text
`String`; 

**get()**

```js
feature.get('text')
// returns: "my line of text"
```

**set()**

```js
feature.set({'text':"my line of text"})
```

**default**

`""`
:::

:::{tab-item} link
`String`; 

**get()**

```js
feature.get('link')
// returns: "https://..."
```

**set()**

```js
feature.set({'link':"https://..."})
```

**default**

`""`
:::

:::{tab-item} fontSize
`Integer`; 

**get()**

```js
feature.get('fontSize')
// returns: 25
```

**set()**

```js
feature.set({'fontSize':25})
```

**default**

`25`

:::{tab-item} color
`String` -hexadecimal; 

**get()**

```js
feature.get('color')
// returns: "#00000"
```

**set()**

```js
feature.set({'color':"#fcba03"})
```

**default**

`"#00000"`
:::

:::{tab-item} background
`String` -hexadecimal; 

**get()**

```js
feature.get('background')
// returns: "#00000"
```

**set()**

```js
feature.set({'background':"#fcba03"})
```

**default**

`"#fffff"`
:::

:::{tab-item} type
`String`;

**get()**

```js
feature.get('type')
/* or */
feature.type

// returns: 'sign'
```
:::
::::



