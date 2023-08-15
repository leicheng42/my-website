(boombox)=
# 扬声器 Boombox
扬声器可让您将声音传输到世界中。要使用扬声器，只需单击它，然后从弹出窗口中选择`Start Broadcasting 开始广播` 。

```{note}
课上进来玩一玩
https://www.voxels.com/spaces/2a1c8451-fc5a-4f00-b7f8-4c6dafc964fc/play
```

![boombox-feature-double.png](https://wiki.cryptovoxels.com/boombox-feature-double.png)
## 编辑器
![boombox_editor_v4.25.png](https://wiki.cryptovoxels.com/boombox_editor_v4.25.png)

### Spatial roll off 空间衰减

当玩家离开音频播放器时声音消失的速度。
值在 0 到 5 之间。

## 脚本属性

::::{tab-set}

:::{tab-item} rollOffFactor
`Double`; Value ranging from 0 to 5

**get()**

```js
feature.get('rolloffFactor')
// returns: 1.6
```

**set()**

```js
feature.set({'rolloffFactor':1.6})
```

**default**

`1`

:::

::::

## How to use?
Click on the Boombox and hit start Broadcasting
![boombox-broadcast.png](https://wiki.cryptovoxels.com/boombox-broadcast.png)

