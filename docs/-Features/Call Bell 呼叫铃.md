(call-bell)=
# 呼叫铃 Call Bell

> 自 4.16 版本以来，该功能已被削，不再可用。
{.is-danger}

呼叫铃外观与[按钮](https://wiki.cryptovoxels.com/features/button)类似，按下时会向 Discord 用户发送消息。

![call-bell-feature.png](https://wiki.cryptovoxels.com/call-bell-feature.png)

## Editor 编辑器

### Discord ID

呼叫用户的 discord ID

## 脚本属性

::::{tab-set}

:::{tab-item} feature.discordId
String.
:::

:::{tab-item} feature.soundId
Integer; the ID of the sound the button makes when clicked. This can be an integer in the range of 0 - 14.
:::

::::