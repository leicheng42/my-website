(nft-model)=
# NFT模型 ｜ NFT-模型

允许您使用 Opensea 链接在世界中显示 3d vox 模型。它有一个内置的 GUI 菜单，显示有关 nft 的信息。


## Editor 编辑器

![editor_5.57.png](https://wiki.cryptovoxels.com/features/[nft-model]editor_5.57.png)

### URL

nft 的 Opensea URL。

如果收藏品是在 cryptovoxels 网站上铸造的收藏品，它将显示一个 GUI 菜单，其中包含 `Buy on Opensea` 按钮。

如果没有不是，它将显示一个信息较少的菜单。

例如
https://opensea.io/assets/0xa58b5224e2fd94020cb2837231b2b0e4247301a6/3247

## 脚本属性

::::{tab-set}
:::{tab-item} url
`String`; Links must be `https://` and must be a link from opensea.
eg: `https://opensea.io/assets/0xa58b5224e2fd94020cb2837231b2b0e4247301a6/3247`

**get()**

```js
feature.get('url')
// returns: "https://..."
```

**set()**

```js
feature.set({'url':"https://opensea.io/assets/0xa58b5224e2fd94020cb2837231b2b0e4247301a6/3247"})
```

**default**

`""`
:::

:::{tab-item} type
`String`;

**get()**

```js
feature.get('type')
/* or */
feature.type

// returns: 'nft-model'
```
:::
::::