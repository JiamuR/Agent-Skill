# Agent-Skill

独立整理、按需使用的 Agent 技能合集。每个技能有自己的目录、说明和版本，可以单独下载使用。

## 技能列表

| 技能 | 当前版本 | 主要用途 | 内容与下载 |
| --- | --- | --- | --- |
| Agent 初始化配置 | v2.1 | 核对 Windows Agent 工作目录、C 盘限制、附件存放，以及配置任务的中断恢复 | [技能说明](skills/agent-workspace-init/SKILL.md) · [使用指南](skills/agent-workspace-init/docs/quickstart.md) · [下载 ZIP](https://github.com/JiamuR/Agent-Skill/releases/download/agent-workspace-init-v2.1/agent-workspace-init-v2.1.zip) |
| 简易化需求撰写 | v3 | 将想法、讨论、录音、数据、截图或旧稿整理成便于业务与 IT 同事讨论的简明需求 | [技能说明](skills/simple-requirement-writing/SKILL.md) · [下载 ZIP](https://github.com/JiamuR/Agent-Skill/releases/download/simple-requirement-writing-v3/simple-requirement-writing-v3.zip) |
| 八字论断与追问 | 2026-10-21 首次收录 | 中文八字咨询与学习引导，先核对资料，再结合反馈作参考性解读 | [技能说明](skills/bazi-consultation/SKILL.md) · [下载 ZIP](https://github.com/JiamuR/Agent-Skill/releases/download/bazi-consultation-2026-10-21/bazi-consultation-2026-10-21.zip) |

## 怎样使用

1. 选择需要的技能，下载该技能的 ZIP 并解压。无需同时安装全部技能。
2. 保留完整技能文件夹，包括 `SKILL.md`、`agents` 及已有的参考资料和模板。
3. 按当前 Agent 应用支持的方式导入，或将完整文件夹提供给能读取本地文件的 Agent。应用应能实际读取技能文件；只有名称或未解压的压缩包不代表技能已加载。
4. 发送对应的调用话术，并按技能说明补充目标和材料。是否支持 `$技能名` 的调用方式，以实际应用为准。

**Agent 初始化配置：**

> 使用「Agent初始化配置skill」，帮我检查并确认工作目录、文件夹用途和 C 盘限制。已有配置请沿用，缺失或需要修改的事项逐项问我；涉及迁移、删除、写入记忆或 agent.md 时，先说明具体方案并取得确认。

**简易化需求撰写：**

> 使用「简易化需求撰写」，把下面的想法和材料整理成一份供业务与 IT 同事讨论的简明需求。先让我选择看初稿，还是逐项确定关键点。

**八字论断与追问：**

> 使用「八字论断与追问」，先介绍可以问的方向，再询问出生资料或现成四柱，用保留术语、白话解释的方式作参考性解读。

## 目录与版本

```text
skills/
├── agent-workspace-init/
│   ├── SKILL.md
│   ├── agents/
│   ├── docs/
│   ├── references/
│   └── templates/
├── simple-requirement-writing/
│   ├── SKILL.md
│   └── agents/
└── bazi-consultation/
    ├── SKILL.md
    ├── agents/
    └── references/
```

各技能独立更新，已有版本号时标签采用 `技能名-v版本号`；
未声明版本号的技能采用 `技能名-发布日期`，不补造版本号。
仓库 `main` 分支保存当前内容，固定版本请到 [Releases](https://github.com/JiamuR/Agent-Skill/releases) 下载对应 ZIP；
GitHub 自动生成的 Source code 包包含整个仓库。

发布包保留提供版本的原始内容。初始化技能的 ZIP 使用英文文件名，文件字节不变。
版本与 SHA-256 见 [更新记录](CHANGELOG.md) 和 [校验值](checksums.sha256)。
需求撰写的 v3 沿用原发布包名称，不表示入口文件声明了该版本号。

## 使用边界与反馈

初始化技能面向 Windows，说明中的盘符和目录属于示例，需要按实际环境确认。技能是操作指引，不能代替宿主权限、记忆机制或磁盘限制。

需求撰写技能侧重业务需求，不代替完整技术设计；Word 交付仍依赖实际文档生成与检查能力。

八字技能用于传统文化学习和参考性交流，不内置历法排盘引擎，不提供确定预言，也不能替代现实判断或专业建议。

可通过 [Issues](https://github.com/JiamuR/Agent-Skill/issues) 提交问题或建议，请说明技能名称、版本、使用环境和可复现现象，避免附带账号凭据或未脱敏的业务资料。

本仓库当前公开提供查看与下载，尚未指定开源许可证。
