<div id="top"></div>

# Live Long & Prosper Skills

**把生活选择与关系困惑，转化为有依据、能执行、可复盘的下一步。**

<p>
  <img src="https://img.shields.io/badge/format-Agent%20Skills-2563eb?style=flat-square" alt="Agent Skills">
  <img src="https://img.shields.io/badge/content-Markdown-339933?style=flat-square" alt="Markdown">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-7c3aed?style=flat-square" alt="MIT License"></a>
</p>

面向日常生活选择与人际关系的个人 Agent Skills 集合。根据当前问题选择技能，每个技能都可以独立使用。

## 目录

- [项目概览](#项目概览)
- [技能与功能](#技能与功能)
- [项目结构](#项目结构)
- [快速开始](#快速开始)
- [使用示例](#使用示例)
- [来源与使用边界](#来源与使用边界)
- [参与贡献](#参与贡献)
- [许可](#许可)
- [致谢与生成说明](#致谢与生成说明)

## 项目概览

这些技能为能够读取文件的 AI 助手提供工作指令和参考材料：先理解本次目标，再按需读取相关模块，区分事实与推断，比较方案并提出行动。

你可以只处理眼前的一件事，也可以主动要求更全面的盘点或逐轮练习。建议应结合个人处境与明确意愿，不要求每次展开全部框架。

## 技能与功能

| 技能 | 适合的问题 | 入口与说明 |
| --- | --- | --- |
| **survival-guide-downturn** · 低增长时代个人生存策略 | 现金流压力、工作与学习、居住与照护、健康与支持、复盘收尾、生活目标及权益事务 | [技能入口](skills/survival-guide-downturn/SKILL.md) · [详细说明](skills/survival-guide-downturn/README.md) |
| **interpersonal-strategy** · 人际社交与亲密关系分析 | 关系困惑、聊天复盘与反复自责、恋爱与择偶、边界与施压识别、利益谈判、逐轮对话演练 | [技能入口](skills/interpersonal-strategy/SKILL.md) · [示例与演练](skills/interpersonal-strategy/references/examples.md) |

共同的工作方式：

- **按问题读取资料**：需要哪个领域，就读取对应参考；只追问会实质改变建议的信息。
- **让判断可以检查**：说明依据、关键未知和替代解释，区分作者观点与技能综合建议。
- **把分析落到行动**：给出可执行的下一步、沟通草稿或练习，并说明何时需要调整。

## 项目结构

```text
live-long-and-prosper-skills/
├── README.md
├── LICENSE
└── skills/
    ├── survival-guide-downturn/
    │   ├── SKILL.md
    │   ├── README.md
    │   ├── LICENSE
    │   └── references/             # 7 个领域模块及 2 个来源辅助模块
    └── interpersonal-strategy/
        ├── SKILL.md
        ├── agents/openai.yaml
        └── references/             # 关系、心理、谈判、来源与演练资料
```

技能索引见上表；每个 `SKILL.md` 内还有按问题选择参考文件的目录。

## 快速开始

1. 克隆仓库，或在 [仓库页面](https://github.com/jialueqian/live-long-and-prosper-skills) 选择 **Code → Download ZIP**：

   ```bash
   git clone https://github.com/jialueqian/live-long-and-prosper-skills.git
   ```

2. 从 `skills/` 中选择需要的完整技能文件夹，放入宿主 AI 工具支持的技能目录。例如，安装生存指南时复制 `skills/survival-guide-downturn/`。

3. 保留技能内部 `SKILL.md`、`references/` 及其他资源的相对位置，在宿主中启用或选择对应技能，然后直接描述问题。

**使用条件：**这些是文档型技能，无需为技能本身安装 Python、Node.js 或模型 SDK。实际使用需要能够读取文件并使用技能指令的 AI 工具；安装路径、登录、模型配置与联网能力以宿主说明为准。

## 使用示例

**生活选择：**

```text
用 survival-guide-downturn 帮我比较留在当前城市和搬到低成本城市的取舍。
我需要保留工作机会，也要考虑家人的照护。
先根据已知信息给初步判断，再列出最影响决定的未知条件。
```

**社交与关系：**

```text
用 interpersonal-strategy 帮我做两周同事交往计划，每天最多15分钟。
我想逐渐熟悉团队，不希望勉强自己参加所有聚会。
```

**逐轮演练：**

```text
用 interpersonal-strategy 扮演刚认识的约会对象。
你先开口，我回复；等我说结束，再反馈我的表达和可以改进的地方。
```

提供相关事实、目标与约束即可；个人案例请先脱敏，不提供密码、验证码或账户密钥。

## 来源与使用边界

技能包含有选择的原创摘要、来源定位和行动设计，不包含电子书、扫描件、整书 OCR 或个人关系档案。具体读取范围和采纳限制见 [生活规划来源](skills/survival-guide-downturn/references/sources-and-evidence.md) 与 [人际策略来源](skills/interpersonal-strategy/references/sources-and-limits.md)。

生存指南当前版本为v3.1.0，人际技能于2026-10-19增补复盘收尾与话术事实约束。改动、定向读取范围与验证限制见 [版本记录](CHANGELOG.md)。

作者观点和公开经验用于启发，不自动成为科学结论或人格诊断。动态政策、医疗、法律与金融信息需要结合实际问题查证；缺少工具或证据时，保留未知并提供核实路径。

生成方案或消息草稿不等于获准替用户购买、签约、提交申请或联系他人。具体操作依用户授权与工具权限执行。

## 参与贡献

欢迎通过 [Issues](https://github.com/jialueqian/live-long-and-prosper-skills/issues) 反馈失效链接、说明不清或遗漏情境，也欢迎提交 [Pull Request](https://github.com/jialueqian/live-long-and-prosper-skills/pulls)。

修改时保持技能可独立使用，检查相对链接与目录；新增观点说明适用条件和限制，新增来源保留原链接及读取范围。个人案例先脱敏，不提交未经授权的第三方原著全文。

## 许可

仓库原创内容采用 [MIT License](LICENSE)。第三方原著、网页和其他材料的权利归各自作者或权利人；MIT 不覆盖第三方原著。

## 致谢与生成说明

感谢提供设计启发的作者与公开经验分享者，具体来源记录在各技能参考模块中。

本 README 的结构由 [eli64s/readme-ai](https://github.com/eli64s/readme-ai) **离线模式生成**，中文内容由 AI 补全并核对。

[返回顶部](#top)
