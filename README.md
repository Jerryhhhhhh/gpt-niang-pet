# GPT 娘 · 雅

一位白发紫瞳、带有龙角与淡紫龙翼的原画风半身伙伴。以安静眨眼、轻颔首和克制的手势陪伴工作，举止儒雅端庄。适用于支持 Pets 的 ChatGPT Work 环境。

**[领养 GPT 娘](https://chatgpt.com/s/sharepet_6ad9cc9be0548191b707c78f5fa5a964)** · **[下载精灵图](assets/gpt-niang-spritesheet.png)** · **[下载发布包](https://github.com/Jerryhhhhhh/gpt-niang-pet/releases/latest)**

![GPT 娘的动作预览](previews/main.gif)

## 使用

在已启用 Pets 的对话中发送：

```text
请领养并选用这个宠物：
https://chatgpt.com/s/sharepet_6ad9cc9be0548191b707c78f5fa5a964
```

领养会在你的宠物库中创建自己的副本。无需运行安装脚本；也可以下载 [PNG 精灵图](assets/gpt-niang-spritesheet.png)，交给兼容该格式的工具使用。可用性取决于客户端是否支持并启用了 Pets。

## 动作

| 状态 | 表现 |
| --- | --- |
| 安静待机 | 轻眨眼，双手交叠 |
| 向右移动 | 朝右转身，从容移动 |
| 向左移动 | 朝左转身，发梢与龙翼轻微跟随 |
| 抬手致意 | 小幅抬手，轻转掌心后收回 |
| 轻颔首致意 | 垂眸、轻轻低头，再恢复平视，身体保持稳定 |
| 轻微关切 | 目光微垂，短暂收敛表情后恢复 |
| 耐心等待输入 | 轻侧头，掌心向上邀请回应 |
| 专注思考 | 目光专注，指尖轻触下巴后放下 |
| 检查与确认 | 视线扫过、微颔首确认 |

另外包含 **16 个顺时针注视方向**，由眼睛与头颈共同表现，腰线保持稳定。

原先的跃起动作已替换为下面这组**轻颔首致意**。为兼容精灵图格式，`pet.json` 中零基索引为 `4` 的动作行（第 5 行）仍使用内部状态名 `jumping`，但实际画面没有腾空跳跃。

![轻颔首致意](previews/courteous-nod.gif)

## 更多预览

- [全部九组动画 GIF](previews/all-states.gif) / [MP4](previews/all-states.mp4)
- [16 方向环视](previews/look-loop.gif) / [方向检查图](previews/look-directions.png)
- [全部帧总览](previews/contact-sheet.png) / [四个代表姿态](previews/four-state-stills.png)

## 文件规格

| 项目 | 值 |
| --- | --- |
| 版本 | 1.0.0 |
| 格式 | 透明 PNG，v2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单格尺寸 | 192 × 208 |
| 有效帧 | 73 |
| 每行帧数 | 6, 8, 8, 4, 5, 8, 6, 6, 6, 8, 8 |

精灵图 SHA-256：

```text
7c1596de5b163a45ca95bb980045afc8363f9c1a0ebb48aab9af67171c3e474c
```

帧序、播放时长和方向约定见 [pet.json](pet.json)，公开验证摘要见 [validation.json](validation.json)，文件校验和见 [SHA256SUMS](SHA256SUMS)。精灵图已通过结构、透明度、帧数、方向盲审、独立视觉复核和 Pets 上传前检查；颔首动作按其静稳语义检查，不要求腾空位移。

## 制作

以创作者提供的人物参考图为基准，通过内置 ImageGen 逐组制作动作与视线，再完成确定性的透明背景处理、对齐、拼接和验证。采用半身构图，让面部与手势在小尺寸下仍能辨认。来源说明见 [CREDITS.md](CREDITS.md)。

## English

GPT Niang · Ya is an elegant anime-style, waist-up dragon companion for Pets-enabled ChatGPT Work clients. It includes nine animation states and sixteen look directions. The original jump has been replaced with a gentle courteous nod. Use the [public adoption link](https://chatgpt.com/s/sharepet_6ad9cc9be0548191b707c78f5fa5a964), or download the validated sprite sheet and frame manifest.
