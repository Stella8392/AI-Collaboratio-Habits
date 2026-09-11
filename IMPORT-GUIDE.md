# 导入与安装指南

## 1. 导入到任意新 AI

### 步骤

1. 把 `prompts/system-prompt.md` 放入新 AI 的自定义指令、System Prompt、项目说明或固定上下文。
2. 把 `prompts/memory-prompt.md` 放入长期记忆区。
3. 第一次对话发送 `prompts/first-calibration-prompt.md`，要求新 AI 复述理解、列待确认项。
4. 上传或复制 `templates/` 和 `checklists/`，让新 AI 在执行任务时引用。

### 建议给新 AI 的首句

```text
请先读取本仓库 README.md、IMPORT-GUIDE.md、prompts/、templates/ 和 checklists/。以后处理我的任务时，优先遵循这些协作偏好、任务模板和安全检查清单。
```

## 2. 安装到 Codex Skills

如果使用 Codex Desktop / Codex CLI，并支持本地 Skills：

1. 找到本机 Codex skills 目录，例如：
   - Windows: `%USERPROFILE%\.codex\skills`
   - macOS/Linux: `~/.codex/skills`
2. 将 `skills/` 下需要的技能文件夹复制进去，例如：

```powershell
Copy-Item -Recurse .\skills\ppt-report-builder "$env:USERPROFILE\.codex\skills\ppt-report-builder"
```

3. 重新打开 Codex 或刷新技能列表。
4. 之后当任务命中场景时，新 AI 应自动或手动引用对应 Skill。

## 3. 不支持 Skills 的 AI 怎么用

把对应 `skills/*/SKILL.md` 当成“操作规范文档”上传或复制给 AI，并告诉它：

```text
以后遇到类似任务时，请先读取并遵循这个 SKILL.md 的流程、输出模板和检查清单。
```

## 4. 公开仓库注意事项

如果该仓库是 public：

- 不要上传内部链接、真实路径、账号、token、cookie、客户/人员信息；
- 不要上传真实业务数据、内部文档原文、未公开 SQL；
- 只保留抽象方法、模板、Prompt 和检查清单；
- 更新前先运行 `checklists/github-public-safety-checklist.md`。

## 5. 更新流程

建议每次有新的稳定习惯时：

1. 先判断是否长期可复用；
2. 去除一次性路径、临时判断、敏感信息；
3. 更新对应 `templates/` 或 `skills/`；
4. 更新 README 的索引；
5. 提交到 GitHub。
