(Move-rotate-scale-Feature)=
# 移动/旋转/缩放一个特征
关于如何改变特征的位置和旋转的页面。

![script-example_move-feature.gif](https://wiki.cryptovoxels.com/script-example_move-feature.gif)
## 1. 位置
有几种方法可以移动一个特征。下面我们将逐个介绍每种方法。

### A. 获取位置
您可以使用以下代码行获取物品的位置：
```js
feature.position
```
它将返回一个类似于 `{x:..,y:..,z:..}` 的 Vector3 对象。

因此，要获取位置的 x、y 或 z 坐标，您可以编写：
```js
feature.position.x
// 或者
feature.position.y
// 或者
feature.position.z
```

### B. 设置位置
您可以使用以下代码行设置物品的位置：
```js
feature.position.set(x,y,z)
// 或者
feature.set({position:[x,y,z]}) // 但现在暂时忽略这一点。请参阅第 4 节。
```
例如：
```js
let myObject = parcel.getFeatureById('myImage') // 获取名为 'myImage' 的特征
setTimeout(()=>{ // 等待 5 秒
  myObject.position.set(4.5,0.75,0.5) // 将名为 'myImage' 的特征移动到 x:4.5，y:0.75，z:0.5
},5000)
```

**只更改一个轴**

现在假设您只想更改一个轴。假设您有一个位置为 `{x:1,y:1,z:1}` 的特征，您希望将其更改为 `y=0.5`。
当然，您可以编写
```js
feature.position.set(1,0.5,1)
```
但是添加不必要的 1 是没有意义的。而且如果您没有其他坐标呢？
在这种情况下，可能更适合写下面的代码之一：
```js
feature.position.x = 5 // 如果要将 x 更改为 5
// 或者
feature.position.y = 0.5 // 如果要将 y 更改为 0.5
// 或者
feature.position.z = 6 // 如果要将 z 更改为 6
```

### C. 实际示例

在这个快速示例中，我们使一个物品每隔 1 秒向左和向右（或南北）移动一次。

```js
let right=true // 作为开关（如果为 true：向左，如果为 false：向右）

setInterval(()=>{ // 启动间隔
	if(right){
  	feature.position.z = feature.position.z + 0.25 // 向左移动（或向北）
    right = !right
  }else{
    feature.position.z = feature.position.z - 0.25 // 向右移动（或向南）
    right = !right
  }
},1000)

```
效果如下：
![script-example_practical_position_example.gif](https://wiki.cryptovoxels.com/script-example_practical_position_example.gif)

## 2. 旋转
与位置一样，有几种方法可以旋转特征。下面我们将逐个介绍每种方法。
> 在使用脚本获取或设置特征的旋转时，请记住旋转角度是弧度，而编辑器中的旋转度量是角度。
.
参考：**360 度**转为**3.14 弧度**，**180 度**转为**~1.57 弧度**。
{.is-warning}

### A. 获取旋转
您可以使用以下代码行获取物品的旋转：
```js
feature.rotation
```
它将返回一个类似于 `{x:..,y:..,z:..}` 的 Vector3 对象。

因此，要获取旋转的 x、y 或 z 坐标，您可以编写：
```js
feature.rotation.x
// 或者
feature.rotation.y
// 或者
feature.rotation.z
```

### B. 设置旋转
您可以使用以下代码行设置物品的旋转：
```js
feature.rotation.set(x,y,z)
// 或者
feature.set({rotation:[x,y,z]}) // 但现在暂时忽略这一点。请参阅第 4 节。
```
例如：
```js
let myObject = parcel.getFeatureById('myImage') // 获取名为 'myImage' 的特征
setTimeout(()=>{ // 等待 5 秒
  myObject.rotation.set(0,1.57,1.57) // 将名为 'myImage' 的特征绕其 y 和 z 轴各旋转 180 度。
},5000)
```

**只更改一个轴**

现在假设您只想旋转一个轴。假设您有一个旋转为 `{x:0.52,y:1.57,z:0.1}` 的特征，您希望将其更改为 `y=3.14`。
当然，您可以编写
```js
feature.rotation.set(0.52,3.14,0.1)
```
但再一次，复制和粘贴先前的旋转数据有什么意义。如果您没有 x 和 z 轴呢？
在这种情况下，根据需要编写以下代码之一：
```js
feature.rotation.x = 0.85 // 如果要将 x 更改为 0.85 弧度
// 或者
feature.rotation.y = 3.14 // 如果要将 y 更改为 pi（360 度）
// 或者
feature.rotation.z = 0.5 // 如果要将 z 更改为 0.5 弧度
```

### C. 实际示例

在这个快速示例中，我们使一个物品每隔 1 秒顺时针和逆时针旋转一次。

```js
let clockwise=true // 作为开关（如果为 true：顺时针，如果为 false：逆时针）

setInterval(()=>{ // 启动间隔
	if(clockwise){
  	feature.rotation.y = feature.rotation.y + 30 // 逆时针旋转
    clockwise = !clockwise
  }else{
    feature.rotation.y = feature.rotation.y - 30 // 顺时针旋转
    clockwise

 = !clockwise
  }
},1000)

```
效果如下：
![script-example_practical_rotation_example.gif](https://wiki.cryptovoxels.com/script-example_practical_rotation_example.gif)

## 3. 缩放

特征的缩放属性与位置和旋转非常相似。

### A. 获取缩放
您可以使用以下代码行获取物品的缩放：
```js
feature.scale
```
它将返回一个类似于 `{x:..,y:..,z:..}` 的 Vector3 对象。

因此，要获取缩放的 x、y 或 z 坐标，您可以编写：
```js
feature.scale.x
// 或者
feature.scale.y
// 或者
feature.scale.z
```

### B. 设置缩放
您可以使用以下代码行设置物品的缩放：
```js
feature.scale.set(x,y,z)
// 或者
feature.set({scale:[x,y,z]}) // 但现在暂时忽略这一点。请参阅第 4 节。
```
例如：
```js
let myObject = parcel.getFeatureById('myVox') // 获取名为 'myImage' 的特征
setTimeout(()=>{ // 等待 5 秒
  myObject.scale.set(5,5,5) // 将缩放更改为大的 5x5x5 物体。
},5000)
```

**只更改一个轴**

现在假设您只想缩放一个轴。假设您有一棵树，其缩放为 `{x:1,y:1,z:1}`，您希望将其更改为 `y=6`，因为树通常具有较好的高度。 (嗨..嗯，我爱你，盆栽)
当然，您可以编写
```js
feature.scale.set(1,6,1)
```
但再一次，复制和粘贴先前的缩放是没有意义的。如果您没有 x 和 z 轴呢？
在这种情况下，因为我们只需要更改一个轴，我们可以使用以下代码之一：
```js
feature.rotation.x = 6 // 如果要将 x 更改为 6
// 或者
feature.rotation.y = 6 // 如果要将 y 更改为 6
// 或者
feature.rotation.z = 6 // 如果要将 z 更改为 6
```

### C. 实际示例

在这个快速示例中，我们使一个物品每隔 1 秒变大一次。

```js
let small=true // 作为开关（如果为 true：变大，如果为 false：变小）

setInterval(()=>{ // 启动间隔
	if(small){
  	feature.scale.set(2.5,2.5,2.5) // 变大
    small= !small
  }else{
    feature.scale.set(1,1,1) // 变小
    small= !small
  }
},1000)

```
效果如下：
![script-example_practical_scale_example.gif](https://wiki.cryptovoxels.com/script-example_practical_scale_example.gif)


## 4. 其他方法。

要设置特征的属性（位置、旋转或缩放），您还可以使用以下代码行：

```js
feature.set({position:[x,y,z]})
// 或者
feature.set({rotation:[x,y,z]})
// 或者
feature.set({scale:[x,y,z]})
```

要正确理解此方法，您必须对 [数组](https://www.w3schools.com/js/js_arrays.asp) 有一定的了解。这是因为我们分配给每个属性的数据是一个数组 `[x,y,z]`。

这种方法的优点是可以在一行内分配多个属性，例如：
```js
feature.set({position:[x,y,z],rotation:[x,y,z]})
// 分配位置和旋转。
```

下面是一个实际示例：
```js
let small=true // 作为开关（如果为 true：向左，如果为 false：向右）

setInterval(()=>{ // 启动间隔
	if(small){
  	feature.set({scale:[2.5,2.5,2.5],position:[4.5,0.75,1.5]}) // 向左移动并变大
    small= !small
  }else{
  	feature.set({scale:[1,1,1],position:[4.5,0.75,0.2]}) // 向右移动并变小
    small= !small
  }
},1000) 
```
效果如下：
![script-example_practical_combined_example.gif](https://wiki.cryptovoxels.com/script-example_practical_combined_example.gif)