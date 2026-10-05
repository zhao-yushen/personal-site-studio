# Personal Site Studio · 个人主站工作室

一个供 Codex 使用的个人主站制作与升级 skill。将简历、项目资料和现有实现转化为有辨识度的个人展示站，兼顾内容结构、景观动效与可用交互。

## 适用任务

- 从真实资料构建个人主站或作品集。
- 合并重复展示，减少多层面板和多余操作。
- 改善视觉叙事、背景动效和内容相关的特色交互。
- 按改动风险审查页面，并在需要时发布或调整访问范围。

流程按请求分流：咨询直接回答，小改动处理对应部分，访问策略修改走独立路径，整体改版才进入完整制作流程。风格、技术与模块根据实际内容选择。

## 安装

将此仓库克隆或下载到 Codex 的 skills 目录，目录名称保留为 `personal-site-studio`：

```text
$CODEX_HOME/skills/personal-site-studio/
```

未设置 `CODEX_HOME` 时，通常使用 `~/.codex/skills/personal-site-studio/`。已有自定义 skills 目录时沿用该目录。确保目录中包含 `SKILL.md`、`agents/` 和 `references/`。

也可在支持 `skill-installer` 的 Codex 中请求：

```text
从 https://github.com/zhao-yushen/personal-site-studio 安装 personal-site-studio。
```

## 调用示例

```text
使用 $personal-site-studio，根据我的简历和作品目录制作个人主站。

使用 $personal-site-studio，精简这个作品集的重复展示，保留现有手机版本。

使用 $personal-site-studio，研究适合当前背景的互动方案，这轮只回答。
```

## 文件导航

| 文件 | 作用 |
| --- | --- |
| [SKILL.md](SKILL.md) | 请求分流、核心流程与结束条件 |
| [内容与设计](references/content-and-design.md) | 材料筛选、内容去重、视觉叙事与技术选择 |
| [交互实现](references/interaction-engineering.md) | 状态同步、动效生命周期、焦点、图表和按需导出 |
| [验证与交付](references/verification-and-delivery.md) | 实际页面审查、按风险验证与局部复测 |
| [发布与访问](references/hosting-and-access.md) | 沿用托管方、版本一致性与受众管理 |
| [agents/openai.yaml](agents/openai.yaml) | Codex 展示名称与默认调用提示 |

## 使用边界

项目事实、素材、公开范围和设备限制来自当前任务。示例数据、概念插画与真实成果保留明确区分。外部发布与访问变更遵循当前用户授权和提供方规则。

现有编辑和导出能力可复用；需要可编辑单文件 HTML 时可按需使用已安装的 `personal-homepage-skill` 运行时，并遵守其许可证。该运行时为可选能力。普通制作、咨询和内容精简可直接按本 skill 的独立指引执行。

## 验证

本 skill 已通过 Skill Creator 格式校验和独立试用。试用在隔离的虚构作品页面中验证了桌面内容合并、操作精简、导航与手机版本保留。实际项目仍需按本轮改动验证对应行为。
