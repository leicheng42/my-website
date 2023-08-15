(Make-a-Vox-Model)=
# 📦 制作 vox 模型

Cryptovoxels具有允许导入.vox和Mega-vox功能的功能。
您可以查看 [voxel库](https://wiki.cryptovoxels.com/voxel-library)，了解vox模型的示例。
接下来，我们将介绍如何制作.vox或mega-vox模型。

![how-to-vox-models-example.png](https://wiki.cryptovoxels.com/how-to-vox-models-example.png)

## 1. 获取MagicaVoxel
MagicaVoxel是用于创建.vox 3D模型的软件。它经常更新，其创建者Ephtracy非常活跃且反应迅速。
- 您可以从以下网址获取：[ephtracy.github.io](https://ephtracy.github.io/)
- 安装该软件。

## 2. 打开MagicaVoxel
**并设置您的画布。**

如果您要创建普通的.Vox文件（用于.VOX功能），则画布的大小必须是 `32x32x32`。
如果您要创建Megavox功能，则画布的大小必须是 `126x126x126`。

您可以像这样更改画布大小：
![magicavoxel_changeto32.png](https://wiki.cryptovoxels.com/magicavoxel_changeto32.png)

## 3. 创建您的vox模型
使用Magica的各种工具，您可以轻松创建您理想的vox模型。该软件有很多快捷键，可能需要一些练习才能熟练运用。

vox模型示例：
![small_lamp.png](https://wiki.cryptovoxels.com/small_lamp.png)

您可以使用右上菜单中的:floppy_disk:图标保存它。

## 4. 上传
您可以将vox模型保存在几个地方。推荐的平台有：

- Cryptovoxels Discord服务器 => [#Files](https://discord.gg/BFxEEGc)
- [Pinata云](https://pinata.cloud/) (IPFS服务)
- [Slate](https://slate.host/) (开源IPFS服务)
- [Dropbox](https://www.dropbox.com/)

## 5. 进入虚拟世界并分享您的作品

前往[您的地块](https://www.cryptovoxels.com/account/parcels)，根据您拥有的文件，放置一个.vox或megavox功能。

然后将可共享的URL粘贴到“URL”字段中。
![how-to-vox-model-example2.gif](https://wiki.cryptovoxels.com/how-to-vox-model-example2.gif)

## 旋转中心

在使用旋转动画时，您可能会注意到vox模型实际上不会围绕其自然中心旋转。

对于打算旋转的vox模型，您应该将中心放置在MagicaVoxel画布的特定坐标上。
对于32x32x32 vox模型，请使用 `x:20` 和 `y:15` 作为真正的旋转中心。
您可以使用[此vox模型](https://wiki.cryptovoxels.com/true_center_rotation_tool.vox)来帮助您获得真正的旋转中心。在此模型中，深蓝色的voxels表示近似的旋转中心，而浅蓝色的表示中心。
![true_center_rotation_32x32x32.png](https://wiki.cryptovoxels.com/true_center_rotation_32x32x32.png)

这种方法的一个不便之处是它会强制您缩小vox模型的大小。