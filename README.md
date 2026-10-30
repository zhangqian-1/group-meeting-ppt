# 硕士组会 PPT Skill

用于讨论、制作和修改科研进展、论文分享及混合汇报 PPT。

- 讨论时只给方案，明确要求制作时才生成文件；局部修改保留其他已确认内容。
- 根据听众、时长和页数组织主线，解释关键方法、图表与公式。
- 默认参考随 skill 提供的老师项目稿，按内容灵活安排布局。
- 完整制作默认只交付可编辑 PPTX 和独立逐页 Word 讲稿。
- 中间文件只保留制作、检查与续改必要的内容，不额外交付过程报告。

## 安装

把仓库中的 `skills/group-meeting-ppt` 整个文件夹复制到个人 skills 目录，例如 `~/.codex/skills/group-meeting-ppt`。如果已设置 `CODEX_HOME`，使用对应的 `skills` 目录。已经安装时，不要盲目覆盖自己修改过的版本。

也可把本仓库中 `skills/group-meeting-ppt` 的 GitHub 链接交给 Codex，要求使用 skill-installer 安装。

## 调用

```text
使用 $group-meeting-ppt，按附件制作硕士组会 PPT，汇报15分钟，共10页，直接完成。
```

也可以说“先讨论思路”“先审大纲”或“只修改第3页”。提供本次真实内容材料，特殊听众、时长、页数和模板要求在消息中说明。显式要求优先于默认规则。

## 目录

```text
skills/group-meeting-ppt/
  SKILL.md                      唯一核心规则
  agents/openai.yaml            调用元数据
  references/teacher-style.md   按需读取的参考说明
  assets/teacher-reference.pptx 原始参考报告
  assets/reference-pages/      五张代表页
```

核心规则只维护在 `SKILL.md`；安装目录是使用副本。维护仓库版本后，同步到自己的安装目录即可，无须再维护一套 AGENTS 规则。

参考素材来自用户提供的学术报告，原有署名见 PPT。它们用于研究内容组织和视觉表达；原稿中的身份、标识、数据与研究结论不自动属于新汇报。

PPTX 和 DOCX 的实际制作、渲染及可编辑性检查，需要运行环境具备相应工具；本 skill 提供工作规则和参考，不包含 PowerPoint/Word 运行时。
