(Click-trigger)=
# 简单的点击触发示例

这里我们介绍一个非常简单的点击触发器示例。

![script_example_click_trigger.png](https://wiki.cryptovoxels.com/script_example_click_trigger.png)

## 1. 放置一个按钮和一个标牌

并将标牌的ID字段设置为'triggerResult'

## 2. 复制并粘贴这个脚本
到按钮的脚本字段中。

```js
let textSign = parcel.getFeatureById('triggerResult')

feature.on('click', e => {
	textSign.set({ text: '点击！' })
})


```

快速刷新，完成！

## 3. 它是做什么的？
第一行
```js
let textSign = parcel.getFeatureById('triggerResult')
```
找到您创建的标牌，并将其插入到变量textSign中。
接下来的部分处理点击事件。
```js
feature.on('click', e => {
	textSign.set({ text: '点击！' })
})
```
它简单地侦听点击事件，一旦按钮被点击，它就会告诉标牌显示"点击！"。

## 它适用于体素模型吗？

是的！您可以将此脚本复制粘贴到体素模型的脚本字段中，它将会起作用！