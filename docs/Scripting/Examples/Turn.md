(Turn)=
# 使体素面对玩家

一个体素模型会选择距离最近的玩家并转身跟随他们。

![turn-to-face.png](https://wiki.cryptovoxels.com/turn-to-face.png)

## 如何使用

1. 创建一个体素模型
2. 分配一个URL（示例外星人：`https://cdn.discordapp.com/attachments/573736707984457738/733461614107426836/aliem.vox`）
3. 添加这个脚本
4. 重新加载地块

## 脚本

```js
setInterval(() => {
  let p = parcel.getPlayers()[0]
  
  if (!p) {
    return
  }

  let v1 = feature.position
  let v2 = p.position
  let angle = Math.atan2(v1.z - v2.z, v1.x - v2.x)

  feature.rotation.y = Math.PI / -2 - angle
}, 200)
```

## 改进

重新设计以2赫兹运行，并使用动画API平滑地在旋转之间进行动画切换。

> 敬礼 MATH.ATAN2！