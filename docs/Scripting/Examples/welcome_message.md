(welcome_message)=
# 欢迎和告别标志
当访客进入/离开你的地块时，向他们表示欢迎或告别！

![welcome-goodbye_example.png](https://wiki.cryptovoxels.com/welcome-goodbye_example.png)

## 步骤

1. 放置两个标志，并将第一个标志的ID设置为`welcometxt`
2. 在第二个标志上放置以下脚本：

```js
let msg = parcel.getFeatureById('welcometxt')

parcel.on('playerenter', event => { 
  msg.set({text:"欢迎"})
  feature.set({text:event.player.name})

  console.log(event.player.name)
})

parcel.on('playerleave', event => { 
  msg.set({text:"再见"})
  feature.set({text:event.player.name})

  console.log(event.player.name)
})
```

## 发生了什么
脚本会检测用户何时进入/离开地块，并检索玩家的名称。
它会显示"欢迎 玩家名称"或"再见 玩家名称"。