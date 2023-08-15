(TicTacToe)=
# 井字游戏

一个井字游戏

![tictactoe.png](https://wiki.cryptovoxels.com/tictactoe.png)

## 如何使用

1. 使用[此链接](https://cdn.discordapp.com/attachments/573736707984457738/733838799150514276/ttt-board.vox)创建井字游戏的体素模型
2. 使用[此链接](https://cdn.discordapp.com/attachments/573736707984457738/733842407073775616/cross.vox)添加交叉的体素模型，并设置ID为`cross`
3. 使用[此链接](https://cdn.discordapp.com/attachments/573736707984457738/733842416276340798/nought.vox)添加零的体素模型，并设置ID为`nought`
3. 将此脚本添加到井字游戏棋盘
4. 重新加载地块

## 脚本

```js
let o = parcel.getFeatureById('nought')
let x = parcel.getFeatureById('cross')

let clones = []
let nought = true

feature.on('click', e => {
  if (clones.length === 9) {
    clones.forEach(c => c.remove())
    clones = []
  }
  
  let c = (nought ? o : x).clone()
  c.position.copyFrom(e.point)
  clones.push(c)
  
  nought = !nought
})
```

## 改进

* 检测赢家并绘制一条线
* 需要两名玩家（一旦多人游戏功能实现）