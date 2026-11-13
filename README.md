# 高审美配图Skill

**作者：Vantage万极 · Skill：`high-aesthetic-image` · MIT 开源**

把文案里的一个观点，变成一张有质感、能看懂的配图。

这套方法提炼自 Vantage万极的日常朋友圈配图实践。先找到观众关心的冲突和后果，再用具体物件、空间关系、材质与光线表达。适合朋友圈、品牌观点、产品价值和商业内容。

![高审美配图示例：被看见，却没有进入候选](assets/shortlist-example.png)

*实生成示例 · 无字概念插画。输入、视觉方案与完整提示词见 [示例](examples/shortlist.md)。*

## 它会怎么做

- 让配图与文案表达同一个问题，用一个清楚的场景承载观点。
- 默认采用高级 3D 编辑插画或电影感商业隐喻，保持配色克制、材质可信、光线有层次。
- 在真实页面本身构成论据时使用截图，并保留来源。
- 尊重用户已有的品牌色、风格、比例和参考图；需要时加入短中文钩子，也支持无字图片。
- 检查实际图片中的语义关系、缩略图效果、文字与视觉细节，再交付最终文件。

开源版专注配图，可用于不同业务主题。它不包含微信账号、定时任务或自动发布脚本。

## 安装

在 Codex 默认个人技能目录安装：

```bash
git clone https://github.com/Aiysae/high-aesthetic-image.git ~/.codex/skills/high-aesthetic-image
```

若自定义了 `CODEX_HOME`，使用对应的 `skills/high-aesthetic-image` 目录。也可以[下载 ZIP](https://github.com/Aiysae/high-aesthetic-image/archive/refs/heads/main.zip)，解压后把文件夹命名为 `high-aesthetic-image`，放入个人技能目录。

仓库根目录即 Skill 目录，包含 [SKILL.md](SKILL.md)、界面元数据、提示词模板和示例。

## 使用

生成配图：

```text
使用 $high-aesthetic-image，为下面这条朋友圈文案生成一张配图。
方图，无字，整体克制、专业、有质感。
文案：产品被很多人看见，却没有进入购买时的候选名单。
```

先讨论方案：

```text
使用 $high-aesthetic-image，为“专业服务的价值需要证据支撑”构思一张配图。
先给我一个视觉方案和完整提示词。
```

按已有品牌风格制作：

```text
使用 $high-aesthetic-image，根据这段产品介绍制作一张 4:5 配图。
以我提供的参考图为风格参考，保留品牌色，画面只突出一个购买理由。
```

## 运行环境

这是一个 Skill 指令包，不捆绑图像模型或 API 客户端。实际生成图片需要宿主提供图像生成能力；在 Codex 中优先使用内置图片工具，无须为了使用本 Skill 单独配置 API Key。工具可用性、额度与费用以使用者自己的环境为准。

纯文本环境可以使用它完成视觉方案和提示词。真实截图路线需要可访问的原始页面或用户提供的素材。

## 方法与验证

执行规则见 [SKILL.md](SKILL.md)，提示词结构见 [模板](references/prompt-template.md)。仓库示例用于展示无字商业场景的生成效果；带字图片仍需逐张检查中文和可读性。

生成式插画用于表达观点。客户评价、数据、真实平台界面和经营结果应来自可追溯的材料。

## 许可证

本 Skill 由 **Vantage万极** 开源，采用 [MIT License](LICENSE)。使用、修改和分发时保留许可证与版权声明。
