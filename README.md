# AI Collaboration Habits / 个人 AI 协作习惯迁移包

这是一个**脱敏版**个人 AI 工作记忆迁移包，用于在更换 AI 模型、账号或电脑时，快速导入长期协作偏好、任务执行模板、检查清单和可复用 Skills。

> 安全说明：本仓库不应包含账号、密码、token、cookie、客户/人员隐私、内部机密原文、真实业务数据、内部链接或不可公开路径。若后续补充内容，请先执行 `checklists/github-public-safety-checklist.md`。

## 新 AI 读取顺序

建议让新 AI 按以下顺序读取：

1. `prompts/system-prompt.md`：长期服务规则，适合放到 System Prompt / 自定义指令 / 项目说明。
2. `prompts/memory-prompt.md`：短版长期记忆，适合放入 Memory 区。
3. `prompts/first-calibration-prompt.md`：第一次对话时让新 AI 复述理解并列待确认项。
4. `IMPORT-GUIDE.md`：了解如何导入、安装 Skills、使用模板。
5. `templates/`：不同任务类型的执行模板。
6. `skills/`：可复制到 Codex / 其他支持 Skills 的 AI 环境中的技能包。
7. `checklists/`：任务收尾、事实边界、敏感信息、公开仓库安全检查。

## 目录结构

```text
prompts/      # 给新 AI 直接复制的 System / Memory / Calibration Prompt
templates/    # PPT、长文档、数据分析、SQL口径、Prompt优化等任务模板
skills/       # Codex 风格 SKILL.md，可作为可复用技能包
checklists/   # 敏感信息、事实边界、GitHub公开安全、任务收尾检查
examples/     # 典型任务流程示例
```

## 最简导入方式

如果新 AI 不支持技能安装，只需要复制：

```text
prompts/system-prompt.md
prompts/memory-prompt.md
prompts/first-calibration-prompt.md
```

如果新 AI 支持知识库上传，请上传整个仓库或压缩包，并要求它优先读取 `README.md` 和 `IMPORT-GUIDE.md`。

## 适合反复复用的任务

- 长文档总结、改写、降 AI 痕迹
- PPT / 汇报材料制作与优化
- 业务方案分析、需求拆解、项目计划
- SQL 指标口径说明、数据分析报告
- 会议纪要整理、风险审查
- Prompt 优化、个人知识库整理、跨模型迁移
- 知识库问答 / RAG 优化
