---
title: [Bind] 如何正确绑定/同步账号
description: 
published: true
date: 2024-12-03T06:19:40.809Z
tags: 
editor: markdown
dateCreated: 2024-12-03T05:48:39.421Z
---

![](https://img.shields.io/badge/Dreamlight-a48bf8?style=for-the-badge&label=Writer)![](https://img.shields.io/badge/Milk-blue?style=for-the-badge)

# Bind详细用法：
1. 首先请确认**你要绑定的平台** 和 **怎么绑定**（你是把QQ数据覆盖到Discord还是把Discord数据覆盖到QQ）

2. 然后找到**你要被覆盖的平台**（目标平台）和带有数据的平台（原始平台）可以使用NyaProxyBot的地方（例如QQ和Discord）

3. 然后在**你想要被覆盖的平台**（目标平台）发送`/bind` 或 `!bind`（DiscordBot使用者请使用!指令）

4. 然后这时候你会收到机器人的消息:
> Bind 指令可用于在多个平台间绑定用户数据。绑定过程中，原始平台的用户数据将完全保留，而目标平台的用户数据将被原始平台的数据所覆盖。
请确认当前平台是你的目标平台，并在 5 分钟内使用你的账号在原始平台内向机器人发送以下文本：
`koishi/424165`
绑定完成后，你可以随时使用「bind -r」来解除绑定状态。
![bind1.png](/bindfaq/bind1.png)
5. 将这个Koishi码发送到你**带有数据的平台**（原始平台） 你会得到第二个 Koishi 码
> 令牌核验成功！下面将进行第二步操作。
请在 5 分钟内使用你的账号在目标平台内向机器人发送以下文本：
`koishi/075609`
注意：当前平台是你的原始平台，这里的用户数据将覆盖目标平台的数据。
![bind2.png](/bindfaq/bind2.png)


6. 将这个Koishi码再发送到你想要被覆盖设备的平台（目标平台） 当 Bot 提示“账号绑定成功！” 你的数据就绑定好了
![bind3.png](/bindfaq/bind3.png)

之后在两方绑定的任意一个平台都可以使用 NyaProxy 数据会实时同步（例如时长 审计日志 使用状况等）
如果你今后想要解除绑定 只需要在你的被覆盖的平台（目标平台）发送“/bind -r”或“!bind -r”（DC使用 !bind -r）即可解除绑定
![bind4.png](/bindfaq/bind4.png)
**如果你绑定后数据丢失** 请检查你想要被覆盖的平台和带有数据的平台绑定是否有问题（例如QQ有数据但QQ成为了目标平台被覆盖 或者Discord有数据但Discord被覆盖） 使用`!bind`解除绑定后重新绑定