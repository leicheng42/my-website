(Simple-Door)=
# 简单的门

一个简单的门，在点击时打开和关闭。
![simple_door_example.gif](https://wiki.cryptovoxels.com/simple_door_example.gif)

## 1. 获取你的门 vox 模型。

**首要事项是，在制作 vox 模型时，请确保旋转中心位于正确的位置。**

- [了解如何制作 vox 模型](https://wiki.cryptovoxels.com/Parcels/Make-Vox-Model)
- [了解实际的旋转中心](https://wiki.cryptovoxels.com/Scripting/Animation-API#center-of-rotation)

为了让你的生活更简单，可以随意使用并修改[我在上面的gif中使用的门模型](https://wiki.cryptovoxels.com/door_edited_centered.vox)。

在编辑模型时，你必须确保保持旋转轴在 `x:20` 和 `y:15`。在我分享的门模型中，它由黑色的体素标示出来。
![simple_door_centered_script_example.png](https://wiki.cryptovoxels.com/simple_door_centered_script_example.png)

## 2. 放置并添加脚本

将你的 .vox 特征放置在世界中（查看[这里](https://wiki.cryptovoxels.com/Parcels/Make-Vox-Model)了解如何放置在世界中或托管你的模型），然后添加以下脚本：
```js
let closed = true

feature.on('click',e=>{

  if(closed){
  		feature.rotation.y=0
  }else{
      feature.rotation.y=1.57   

  }
closed=!closed
})
```

## 3. 自定义
- 如果 **第2步** 中的脚本打开门而不是关闭门，只需将第1行中的 `closed` 改为 `false`。

- 如果你想部分打开门，而不是完全打开它，请更改 `open` 角度。所以，如果你的门在弧度角为0时打开，将其更改为0.5或-0.5，这取决于它是推拉门。这可能需要一些试错。

玩得开心！