# Creating Viral Short Dramas

一个面向 Codex、Claude Code 和其他兼容 Agent Skills 规范运行时的中文短剧编排 Skill。它将短剧开发、可拍剧本、前三秒钩子、留存节奏与中文网感润色按任务需要组合起来。

## 适用场景

- 从一个点子开发竖屏短剧、漫剧或剧情短视频
- 写、续写或局部修改一集可拍剧本
- 设计前三秒钩子，并逐一核对承诺是否在剧情中兑现
- 去翻译腔、保留角色声音地润色中文台词
- 审查既有剧本的因果、钩子、人物动机和可拍性

## 核心原则

故事契约优先于流量套路。每个交付给用户的钩子——包括备选——都必须标明能证明其字面承诺的具体兑现节拍；不能兑现就降级、改写或删除。

这是一个编排层，不复制或打包上游 Skill 的内容。请先安装以下依赖，并遵守各仓库的许可：

- [Drama Skills](https://github.com/zenstory-ai/drama-skills)：`short-drama-develop`、`short-drama-write`、`short-drama-review`
- [Vyral Content Skills](https://github.com/vyralcontent/content-skills)：`viral-hooks`、`viral-short-form`
- [Spellbook](https://github.com/majiayu000/spellbook)：`xiaohongshu-netfeel-guardian`

## 安装

将本仓库克隆或复制到运行时的 Skills 目录。例如 Codex：

```text
~/.codex/skills/creating-viral-short-dramas/
├── SKILL.md
└── agents/
    └── openai.yaml
```

随后直接描述任务，或调用：

```text
$creating-viral-short-dramas
```

## 状态

实验性 Skill。结构验证已通过；正式投放前仍应人工核对每一个候选钩子的“承诺—兑现”对应关系。

## License

[MIT](LICENSE)
