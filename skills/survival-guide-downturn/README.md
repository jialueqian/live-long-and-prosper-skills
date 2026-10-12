<div id="top">

# 低增长时代个人生存策略

<em>稳住基本生活，理清重要取舍，为自己保留有价值的选择。</em>

<p>
  <img src="https://img.shields.io/badge/version-3.0.1-2563eb?style=flat-square" alt="Version 3.0.1">
  <img src="https://img.shields.io/badge/format-Agent%20Skill-339933?style=flat-square" alt="Agent Skill">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-7c3aed?style=flat-square" alt="MIT License"></a>
</p>

**survival-guide-downturn** · 现金流 · 工作与居住 · 健康与照护 · 关系支持 · 人生方向

## 目录

- [项目概览](#项目概览)
- [主要功能](#主要功能)
- [项目结构](#项目结构)
  - [文件索引](#文件索引)
- [快速开始](#快速开始)
  - [使用条件](#使用条件)
  - [安装](#安装)
  - [使用](#使用)
- [典型问法](#典型问法)
- [来源与使用边界](#来源与使用边界)
- [常见问题](#常见问题)
- [参与贡献](#参与贡献)
- [许可](#许可)
- [致谢与生成说明](#致谢与生成说明)

---

## 项目概览

这是一个用 Markdown 编写的 Agent Skill，供 AI 助手在经济下行、收入不稳或人生转折中提供生活规划与决策支持。它帮助你结合现实约束比较方案，确定下一步，并在情况变化时复盘。

你可以只解决眼前的一件事，也可以主动发起全面生活盘点。安稳、成长、陪伴、休息都可以成为目标，取舍以你的处境和意愿为起点。

> 低增长是需要考虑的背景，不是对每个人未来的预言。这里的框架用于帮助判断，不能保证某种人生结果。

## 主要功能

| 领域 | 可以获得的帮助 |
| --- | --- |
| **生活方向** | 说清想改善什么、怎样才算够用，以及哪些代价不能接受。 |
| **财务与保障** | 找出现金流缺口，比较债务、住房、储备、保险与照护安排。 |
| **工作与选择** | 分析失业应对、辞职、副业、技能投入和迁居的实际成本。 |
| **关系与支持** | 梳理共同责任、个人边界、可获得的帮助和沟通方式。 |
| **健康与注意力** | 调整行动负担、休息与精力安排，整理需要专业支持的问题。 |
| **宏观背景** | 在与当前决定有关时，辨别宏观变化可能产生的具体影响。 |
| **权益与事务** | 整理欠薪、救助、防骗、照护及身后事务的材料与待核事项。 |

七个领域按需调用，另有来源记录与公开经验两个辅助模块。具体问题先处理相关部分，全面盘点才扩展范围；未知信息保留为未知。

## 项目结构

```text
survival-guide-downturn/
├── SKILL.md
├── README.md
├── LICENSE
└── references/
    ├── life-design.md
    ├── finance-and-insurance.md
    ├── work-and-options.md
    ├── relationships-and-support.md
    ├── health-and-attention.md
    ├── macro-context.md
    ├── rights-and-affairs.md
    ├── sources-and-evidence.md
    └── field-notes.md
```

### 文件索引

发布内容共 **12 个文件**：技能入口、项目说明、许可，以及 9 个参考模块。

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](SKILL.md) | 技能入口、按需读取规则与共同判断原则。 |
| [life-design.md](references/life-design.md) | 生活目标、够用标准、决策节奏与取舍。 |
| [finance-and-insurance.md](references/finance-and-insurance.md) | 现金流、债务、住房、储备与保障。 |
| [work-and-options.md](references/work-and-options.md) | 工作、技能、副业、居住与跨境选择。 |
| [relationships-and-support.md](references/relationships-and-support.md) | 关系支持、边界、共同责任与沟通。 |
| [health-and-attention.md](references/health-and-attention.md) | 精力、注意力、休息与专业求助。 |
| [macro-context.md](references/macro-context.md) | 宏观背景与个人决定的关联。 |
| [rights-and-affairs.md](references/rights-and-affairs.md) | 权益救济、反诈、照护与办事准备。 |
| [sources-and-evidence.md](references/sources-and-evidence.md) | 来源定位、核验范围与证据使用。 |
| [field-notes.md](references/field-notes.md) | 公开经验、适用条件及访问限制。 |

## 快速开始

### 使用条件

仓库本身只有文档文件，**使用本技能无需安装 Python、Node.js 或模型 SDK**。你需要一个能够读取这些文件并使用技能指令的宿主 AI 工具。

具体加载方式依宿主而定；联网、账户和模型配置也由宿主提供。本技能可独立使用，不要求额外安装其他技能。

### 安装

1. 使用 Git 下载仓库，或在 [仓库页面](https://github.com/jialueqian/live-long-and-prosper-skills) 选择 **Code → Download ZIP**：

   ```bash
   git clone https://github.com/jialueqian/live-long-and-prosper-skills.git
   ```

2. 从仓库中取出完整的 `skills/survival-guide-downturn/` 文件夹，放入宿主工具支持的技能目录。如果使用单独的技能包，则取出其中的 `survival-guide-downturn/` 文件夹；安装位置及启用方式以宿主说明为准。

3. 保留 `SKILL.md` 与 `references/` 的相对位置，然后在宿主中启用或选择本技能。

### 使用

直接描述问题、目标和已知约束。例如：

```text
使用 survival-guide-downturn 帮我比较是否辞职。
我希望减少加班，但还要承担房租和家人的照护费用。
先根据已有信息给一个初步方案，再指出最影响判断的未知条件。
```

```text
问题与目标 → 确定范围及紧迫事项 → 按需读取模块
           → 比较方案与代价 → 下一步与复盘条件
```

回答通常围绕四件事展开，形式和详细程度随问题调整：

1. **当前判断**：想改善什么，哪些已知，哪些未知会改变建议。
2. **可行选择**：收益、金钱与时间成本、执行负担及失败后果。
3. **下一步**：现有资源内能做的行动、先后顺序和替代路径。
4. **复盘条件**：何时观察什么，以及情况变化后怎样调整。

简单问题可以几句话解决。现金储备、试错投入和等待时间依据个人约束确定；休息、稳定工作、合作和求助都可以是有效行动。

## 典型问法

| 场景 | 可以这样问 |
| --- | --- |
| 短期现金压力 | “失业了，储蓄还能撑两个月，家里还有老人要照顾，先做什么？” |
| 职业选择 | “稳定工作和自由职业怎么比较？我希望留出更多陪家人的时间。” |
| 迁居 | “想去生活成本低的城市，但担心照护和医保衔接，应该先核实什么？” |
| 家庭分工 | “家里的照护几乎都由我承担，怎样结合各人的实际能力讨论分工？” |
| 全面盘点 | “帮我盘点现在的生活。我最想改善的是睡眠和时间，不急着增加收入。” |

可以提供金额区间、已知截止日期和不能接受的代价。无需一次填写完整问卷，也不要提供密码、验证码或账户密钥。

## 来源与使用边界

**来源可以追溯，读取范围有记录。** v3.0.1完成33份材料的目录筛选和版本指纹记录，对9本EPUB的指定章节/小节及2份扫描PDF的指定原页作正文归因复核；其余22份逐项记录未采用理由。没有通读33份材料。完整定位、阅读范围、取舍与“当前建议—原文—条件—改写”核对表见 [来源记录](references/sources-and-evidence.md)，公开经验及访问失败记录见 [field-notes.md](references/field-notes.md)。

本补丁修正够用三问与实际时薪的章节归因、Money题图与正文定位，补齐杠铃例子、单身生活建议和宏观框架的条件。现金池、情境表、试验流程与话术明确为技能原创或综合设计；保留技能名、调用方式和9个参考模块，不增加运行依赖。

**经验提供启发，结论需要对应证据。** 技能区分用户事实、官方规则、研究、作者观点、网友经验与综合建议。框架和案例不自动成为普遍有效的定律，同一作者的书与文章也不算独立验证。

**动态事实在使用时核验。** 政策、产品条款、金额、资格、程序期限和援助号码，需要按当前地区查证；缺少联网或工具时，应说明未核验事项并给出核实路径。

**规划支持与操作各有边界。** 本技能不能替代诊断、处方、法律代理或个性化投资执业服务。转账、购买、投保、签约、提交申请或联系第三方，需要用户明确授权并符合工具权限。即时人身危险或基本生活无法保障时，先处理紧迫需要。

安装包不含电子书、扫描件或原著全文。

## 常见问题

**需要配置 API Key 吗？**

技能文件本身不需要专用 API Key。宿主 AI 工具可能有自己的登录、订阅或模型配置要求。

**没有联网还能用吗？**

可以基于你提供的信息梳理目标、比较假设情景和准备行动。涉及当前政策、资格或产品事实时，需要补查，无法核验的部分保留为未知。

**每次都要全面盘点吗？**

不需要。直接提出具体问题即可；只有你希望全面盘点时才逐步扩展范围。单纯解释宏观术语，也不会自动启动人生评估。

## 参与贡献

欢迎通过 [Issues](https://github.com/jialueqian/live-long-and-prosper-skills/issues) 反馈说明不清、失效链接或遗漏情境，也欢迎提交 [Pull Request](https://github.com/jialueqian/live-long-and-prosper-skills/pulls) 改进文档。

新增建议请说明适用条件与局限；新增来源请保留原链接、读取范围和核验日期。修改后检查相对链接、文件结构及相关示例是否与技能指令一致。

涉及个人案例时先脱敏，不提交账户信息、密钥或无授权的第三方原著全文。

## 许可

仓库原创结构与内容采用 [MIT License](LICENSE)，Copyright © 2026 jialueqian。

书籍与公开网页的权利归各自作者或权利人。原创摘要、来源定位与链接不改变第三方原著的权利归属；MIT 许可不覆盖第三方原著。

## 致谢与生成说明

感谢提供设计启发的作者与公开经验分享者，具体来源及适用限制记录在参考模块中。

本 README 的结构由 [eli64s/readme-ai](https://github.com/eli64s/readme-ai) **离线模式生成**，中文内容由 AI 补全并核对。

[返回顶部](#top)

</div>
