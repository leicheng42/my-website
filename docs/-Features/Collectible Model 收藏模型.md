# NFT模型 Collectible model

3D显示加密体素收藏品。它有内置的用户界面窗口显示关于NFT的信息。

![example_v7.18.png](https://wiki.cryptovoxels.com/features/[collectible_model]example_v7.18.png)

## Editor 编辑器

![editor_v7.18.png](https://wiki.cryptovoxels.com/features/[collectible_model]editor_v7.18.png)


## 脚本属性

::::{tab-set}

:::{tab-item} collectible
`Object`; An object with multiple properties.
Properties:
```js
{
  chain_id: number
  id: string
  token_id: number
  collection_id: number
  quantity?: number
  name: string
  description?: string
  hash: string
  author: string
  collection_name?: string
  collection_address?: string
}
```

The hash is used to render the vox-model.

**get()**

```js
feature.get('collectible')
// returns: [Object Collectible]
```

**set()**

```js
feature.set({'collectible':myCollectible}) // myCollectible being a collectible object.
 ```

**default**

`null`
:::

:::{tab-item} type
`String`;

**get()**

```js
feature.get('type')
/* or */
feature.type

// returns: 'collectible-model'
```
:::
::::