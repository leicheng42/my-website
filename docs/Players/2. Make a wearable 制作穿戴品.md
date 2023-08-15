(Create-a-wearable)=
# 制作穿戴品

## 1. 要求

穿戴品位于[集合](https://wiki.cryptovoxels.com/en/Player_customization/Create_a_wearable#h-3-collections)中，为了创建一个集合，您需要拥有一个[地块](https://wiki.cryptovoxels.com/en/Parcels/Buy-a-parcel)。
如果您没有拥有地块，您可以选择[提交到公共集合](https://wiki.cryptovoxels.com/en/Player_customization/Create_a_wearable#submit-to-a-public-collection)，或者请拥有地块的人为您创建一个集合。
> 您只允许在拥有地块的情况下创建一个集合。
{.is-warning}

您还需要使用Matic或ETH（取决于集合）来进行每笔交易。
最后，穿戴品必须符合社区准则 - 不能包含冒犯性、种族主义、歧视性、支持暴力或不适宜内容。

## 2. 创建一个vox模型
### 使用MagicaVoxel
要创建vox模型，您需要 [MagicaVoxel](https://ephtracy.github.io/) 软件。下载最新版本，安装它，然后打开。

第一步是将大小设置为32x32x32 - 您可以通过在右上角选择40s，然后输入32并按回车键来实现这一点。

![magica_size.png](https://wiki.cryptovoxels.com/createawearable/magica_size.png)

现在，您可以使用MagicaVoxel来创建自己的帽子、滑雪板、T恤等穿戴品。

> 在制作物品时，尺寸和旋转并不重要，因为所有者在佩戴时可以重新调整和旋转穿戴品 - [点击这里查看用户如何佩戴和自定义穿戴品](https://wiki.cryptovoxels.com/Player_customization/Costume_tab)。
{.is-info}

### 保存您的vox文件

完成您的穿戴品制作后，请保存它。

![magica_save.png](https://wiki.cryptovoxels.com/createawearable/magica_save.png)

确保画布大小为32x32x32！

### 上传您的穿戴品
您的物品已经创建好了，现在是时候将其上传进行审核了！

**您有两个选择：**
1. [将您的穿戴品铸币到您的集合中](https://wiki.cryptovoxels.com/en/Player_customization/Create_a_wearable#minting-a-wearable)（您需要[先创建一个集合](https://wiki.cryptovoxels.com/en/Player_customization/Create_a_wearable#creating-a-collection)）
2. [将您的穿戴品提交到公共集合](https://wiki.cryptovoxels.com/en/Player_customization/Create_a_wearable#submit-to-a-public-collection)

选择2而不是1的优点是，您可以让其他人管理集合，并且这个人必须支付铸币费用。
然而，集合所有者还有资格获得OpenSea交易的版税费用。

### 提示、脚本和教程
MagicaVoxel允许使用脚本（着色器），可以导入某些文件类型以简化创建过程，并且可以加载颜色调色板，并轻松创建渐变效果。

#### 导入
要导入PNG或JPG，请将其拖放到MagicaVoxel中（先清除画布）。例如，您可以导入像素艺术面孔，然后按照您的喜好拉伸它。如果您选择这种方式，您可能需要预先将其缩小到32x32（如果在Photoshop中进行，请确保使用Nearest Neighbor进行重新采样）。

![magica_import_png.gif](https://wiki.cryptovoxels.com/createawearable/magica_import_png.gif)

要导入OBJ，请将其拖放到MagicaVoxel中。导入文件时，MagicaVoxel可能会包含一个隐藏的图层，您必须删除它 - 否则无法将vox导入到Cryptovoxels中。请查看下面的GIF以了解如何删除。

![magica_import_obj.gif](https://wiki.cryptovoxels.com/createawearable/magica_import_obj.gif)

#### 着色器和颜色
着色器放在着色器文件夹中，调色板放在调色板文件夹中。在加载了一些着色器之后，可以从右侧面板或底部的控制台访问它们。[这个网站](https://mode-vis.gumroad.com/?sort=newest)提供了许多不同的着色器供您使用。

![magica_shaders.png](https://wiki.cryptovoxels.com/createawearable/magica_shaders.png)

为了创建渐变效果，按住CTRL+ALT，然后单击/按住起始颜色，并将其拖到结束颜色。

![magica_gradient.gif](https://wiki.cryptovoxels.com/createawearable/magica_gradient.gif)

#### 在铸币之前试穿
虽然没有官方功能可以在铸币之前先试穿穿戴品，但您可以将vox放在您的地块（或沙盒地块）上，然后走进去进行模拟。

在放置vox并调整位置/缩放/旋转后，按C键进入第三人称并走进去。这不是完美的，但是可以使用。

![trying_it.gif](https://wiki.cryptovoxels.com/createawearable/trying_it.gif)

查看[定制](https://wiki.cryptovoxels.com/Player_customization/Costume_tab)部分，了解玩家如何在自己身上佩戴穿戴品的所有方法。

#### 让其他人试穿
如果您的穿戴品已经铸币并且在您的钱包中，您可以允许其他人在购买前

试穿。

1. 按下*TAB*键或点击右上角的方块
2. 选择**Collectible Model**并将其放置在您的地块上
3. 从**Your Collectibles**中选择穿戴品
4. 选中**Allow parcel visitors to try on collectible**复选框
5. 选择**Bone**
6. 调整**position** / **rotation** / **scale**
7. 测试一下，确保您看起来很好

![trying_it2.gif](https://wiki.cryptovoxels.com/createawearable/trying_it2.gif)

#### 故障面部效果
[Stella](https://www.cryptovoxels.com/avatar/0xf1182c5e5bcd7c90b04eb14eb4f971c52f510d47) 发现了一种在Cryptovoxels中制作令人惊叹的故障穿戴品的方法。 😸
![glitchedface.gif](https://wiki.cryptovoxels.com/createawearable/glitchedface.gif)
要复制这个疯狂的效果，请查看[此处的教程](https://www.youtube.com/watch?v=Frn3JCyWHY4)！

#### 扁平穿戴品
如果您计划制作扁平或薄的穿戴品，您必须在MagicaVoxel中以某种特定方式创建它，否则缩放可能会出现问题。下面您可以看到三个不同的VOX文件，看起来相似，但在缩放时，其中一个明显不一样（并随之移动）。

![flat3.gif](https://wiki.cryptovoxels.com/createawearable/flat3.gif)

为了确保您的扁平穿戴品在缩放时不会出现问题，请在“地面”上创建它，或者将其放在中心点，如下所示（即y:15）。

![flat.png](https://wiki.cryptovoxels.com/createawearable/flat.png)

#### 教程
如果您对MagicaVoxel完全不熟悉，或者想深入了解更多信息，请查看这些资源：

- [初学者写作指南](https://www.raywenderlich.com/375-magicavoxel-3d-art-tutorial)
- [快速入门视频](https://www.youtube.com/watch?v=J5fK79E_RXE)（图标来自较旧版本）
- [详细视频](https://www.youtube.com/watch?v=uKOBIHSgIwI)（忽略渲染部分）
- [官方资源](https://ephtracy.github.io/index.html?page=mv_resource)（有很多好东西）

## 3. 集合
集合是一组3D NFT，可在虚拟世界中生成或穿戴。

在Cryptovoxels中创建并列入白名单的集合意味着您可以基于区块链创建自己的品牌收藏品（在这种情况下为穿戴品）。

玩家可以佩戴或放置该集合的收藏品在虚拟世界中。他们还可以在Cryptovoxels网站和OpenSea上找到您的集合和收藏品。您还可以通过Cryptovoxels和OpenSea管理您的集合的各个方面。

> 拥有地块的玩家允许创建一个集合。如果您没有拥有地块，则必须提交到公共集合。
拥有的地块大小不会决定您可以在集合中拥有的穿戴品数量。
{.is-warning}

### 创建一个集合
1. 使用您的钱包登录Cryptovoxels，点击顶部菜单栏上的 [Marketplace](https://www.cryptovoxels.com/marketplace) 
1. 点击 [Collections](https://www.cryptovoxels.com/collections)
1. 点击**Make your own!**
1. 点击**Create a collection**

![create_collection.png](https://wiki.cryptovoxels.com/createawearable/create_collection.png)

5. 点击**Create a collection**按钮

![create_eligibility.png](https://wiki.cryptovoxels.com/createawearable/create_eligibility.png)

6. 选择**Chain Id**并点击**Next**按钮

![select_a_chain.png](https://wiki.cryptovoxels.com/createawearable/select_a_chain.png)

7. 您的钱包可能会要求您切换网络，因此点击**Switch network**（如果您没有看到此消息，请忽略）

![switch_network.png](https://wiki.cryptovoxels.com/createawearable/switch_network.png)

8. 填写集合的信息，点击**Save & Next**按钮（您可以随时通过**⚙Admin**页面修改名称、描述和标志）

![collection_info2.png](https://wiki.cryptovoxels.com/createawearable/collection_info2.png)

9. 命名合约，点击**I assert…**复选

框和**Upload And Deploy**按钮继续

10. 您将需要Matic（或根据集合不同可能是ETH）在Matic Mainnet上（或以太坊主网上）进行下一步操作，所以一旦您有一些可用的，请点击**Confirm**

![confirm_transaction.png](https://wiki.cryptovoxels.com/createawearable/confirm_transaction.png)

11. 成功部署后，将弹出确认窗口

![deployed_contract.png](https://wiki.cryptovoxels.com/createawearable/deployed_contract.png)

12. 填写缺失的信息

![collection_info.png](https://wiki.cryptovoxels.com/createawearable/collection_info.png)

13. 在添加所需信息后，点击复选框，然后点击**Submit**按钮

14. 所有文本应该已经清除，出现了带有绿色背景的消息 - 点击链接，其中写着**Click here to see it!**

15. 现在您应该看到您的集合 - 点击**⚙Admin**按钮并将该页面加入书签

![admin.png](https://wiki.cryptovoxels.com/createawearable/admin.png)

恭喜 - 您现在拥有一个集合！

> 您的所有集合（和收藏品）可以在[这里](https://www.cryptovoxels.com/account/collectibles)找到。
{.is-info}

### 铸造一件穿戴品
现在您已经准备好铸造了！转到您的集合页面，并确保您已登录（它应该类似于https://www.cryptovoxels.com/collections/1）。
如果您要提交到公共集合，请跳过下一节。

> 计划铸造鞋子或需要用户拥有两个穿戴品的其他物品？请记住，**用户需要拥有两个您的穿戴品**（这意味着您可能需要铸造双倍数量）。此更改是在2021年11月左右进行的。
{.is-warning}

#### Polygon/Matic RPC
为确保稳定性，建议将您的钱包的Polygon/Matic RPC切换到https://rpc-mainnet.maticvigil.com/。

![rpc.png](https://wiki.cryptovoxels.com/createawearable/rpc.png)

#### 上传到您的集合
![mint.png](https://wiki.cryptovoxels.com/createawearable/mint.png)

1. 点击**🏭Mint**按钮。
2. 输入**Name**和**Description**（不要触摸Owner信息）
3. 设置**Issues**的数量
*稀有度：1–9 传奇 | 10–99 史诗 | 100–999 稀有 | ≥1000 普通*
4. 点击**Choose File**按钮并选择您的vox文件
5. 点击同意TOS的复选框
6. 点击**Submit**按钮
7. 滚动到下面，您的提交将显示在*Collectible submissions*下面 - 如果您没有看到它，请点击**Refresh**按钮
8. 检查预览是否显示动画gif

![gif_before.png](https://wiki.cryptovoxels.com/createawearable/gif_before.png)

9. 如果显示错误，请点击操作下方的**Refresh gif**按钮。之后将出现以下窗口：

![gif_refresh.png](https://wiki.cryptovoxels.com/createawearable/gif_refresh.png)

10. 如果收到**ok**，刷新浏览器，然后再次点击**🏭Mint**并向下滚动查看提交

![gif_fixed.png](https://wiki.cryptovoxels.com/createawearable/gif_fixed.png)

11. 如果一切正常，请点击**Mint**。如果出现问题，请点击**Reject**。

12. 如果您铸造了它，您的钱包将弹出以确认交易，这将需要极少量的Matic（或ETH） - 点击确认以继续铸造。

![token_id.png](https://wiki.cryptovoxels.com/createawearable/token_id.png)

13. 在*Collectible submissions*下面，将会有一个右侧的链接，上面写着**Collectible ready** - 点击它

![collectible_ready.png](https://wiki.cryptovoxels.com/createawearable/collectible_ready.png)

14. 现在您应该在Cryptovoxels页面上看到您的穿戴品

![mint_success.png](https://wiki.cryptovoxels.com/createawearable/mint_success.png)

恭喜，您刚刚铸造了您的第一件穿戴品！

> 前往[此处](https://wiki.cryptovoxels.com/Player_customization/Costume_tab)了解如何佩戴穿戴品。
{.is-info}

#### 提交到公共集合
如果您没有拥有地块，您可以随时提交到公共集合。

1. 前往https://www.cryptovoxels.com/collections
2. 点击**Available to public**复选框
3. 选择一个集合
4. 点击**🏭Submit**按钮

![public_collection.png](https://wiki.cryptovoxels.com/createawearable/public_collection.png)

5. 阅读警告，填写信息，然后点击底部的复选框，最后点击**Submit**按钮
6. 您现在必须等待由集合所有者批准 - 您可能希望通过Cryptovoxels / Discord向他们发送消息
7. 一旦集合所有者铸造了穿戴品，您将在Cryptovoxels上收到一条消息（如果您收到了它，顶部的**Inbox**旁边将会出现一个红点）

### 交易穿戴品
您可以在Cryptovoxels网站或OpenSea上进行穿戴品的转移。

#### 在Cryptovoxels上交易
要使用Cryptovoxels网站进行转移，请前往要发送的穿戴品的页面[例如https://www.cryptovoxels.com/collections/

1/item/10](https://www.cryptovoxels.com/collections/1/item/10)然后点击**⚙Owner**按钮。从下拉菜单中选择**Transfer…**。输入接收者的地址，然后点击**Submit**按钮。

![transfer_cryptovoxels.png](https://wiki.cryptovoxels.com/createawearable/transfer_cryptovoxels.png)

#### 在OpenSea上交易
在OpenSea上交易时，您可以让您的穿戴品显示在您的个人资料页面或隐藏。在个人资料页面上，单击穿戴品，然后选择**Sell**按钮。填写交易信息，并确定您要进行的出售方式（拍卖或固定价格）。然后点击**List Item**按钮。

![sell_opensea.png](https://wiki.cryptovoxels.com/createawearable/sell_opensea.png)

## 4. 审核
目前，Cryptovoxels并没有提供一个简单的审核系统 - 相反，需要在 [Discord服务器](https://discord.gg/hJmKqsw)上人工提交审核请求。

1. 加入Discord服务器
2. 转到**#wearables**频道
3. 发送一个消息来请求审核。

示例消息：
```
Hello! I've created a new wearable and I would like to get it reviewed for approval. Here are the details:

Collection: My Awesome Collection
Name: Cool Hat
Description: A really cool hat for stylish avatars
Issues: 1000 (rarity: common)
File: [link to the vox file]

Thank you!
```

等待一个管理员审核您的请求。如果您的穿戴品被接受，您将获得一条确认消息。

> 如果您发现有需要解决的问题，请在反馈中尽量提供详细信息，这样管理员才能更容易帮助您。

## 5. 重复
您可以一次性铸造许多穿戴品，并且一旦您的集合获得审核，您就可以在Cryptovoxels中持续铸造。您还可以创建多个集合，以便针对不同的穿戴品类型或主题组织它们。

祝您好运，期待看到您在Cryptovoxels中的创作！