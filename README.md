# course-paper-writer-zh

面向中文大学通识课、选修课及非学位性质结课论文的 Codex Skill。

它把宽泛的课程主题转化为可执行的论文流程，覆盖选题收窄、文献检索、证据核验、论证框架、正文写作、自然化修改和提交前检查，并支持 GB/T 7714—2025 参考文献著录。

## 特点

- 从课程名或宽泛主题缩小到可回答的研究问题；
- 用锚点文献、引用链和证据矩阵组织材料；
- 区分已核实全文、仅见摘要、二手来源和待核信息；
- 禁止虚构作者、页码、DOI、数据及直接引语；
- 根据教师模板、学校规范和用户要求选择格式；
- 支持顺序编码制和著者—出版年制；
- 覆盖网页、数据集、预印本等 GB/T 7714—2025 类型。

## 安装

将仓库克隆到 Codex 用户技能目录：

```powershell
git clone https://github.com/shixiliya1/course-paper-writer-zh.git "$env:USERPROFILE\.codex\skills\course-paper-writer-zh"
```

也可以克隆到某个项目的 `.agents/skills/course-paper-writer-zh` 目录，作为项目级 Skill 使用。

## 使用

在 Codex 中调用：

```text
使用 $course-paper-writer-zh，帮我把“数字时代的文化传播”缩小成一篇 4000 字课程论文的选题和提纲。
```

```text
使用 $course-paper-writer-zh，按 GB/T 7714—2025 核验并修订这些参考文献。
```

如果教师提供任务书、评分标准或模板，请一并交给 Codex。Skill 会优先遵循课程的明确要求。

## 目录

```text
course-paper-writer-zh/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── format-and-qc.md
    ├── gbt7714-2025.md
    └── research-and-writing.md
```

## 关于 GB/T 7714—2025

仓库仅包含面向课程论文场景的原创规则摘要和工作流程，不分发国家标准原文。遇到疑难著录项目时，应查阅合法取得的正式标准文本，并以教师、学院或投稿模板指定的版本为准。

## 学术诚信

本 Skill 用于辅助研究和写作，不代表课程允许使用生成式 AI。使用者应遵守所在学校和课程的规定，亲自核验来源、引文和最终提交内容，并按要求披露 AI 使用情况。

## License

[MIT](LICENSE)
