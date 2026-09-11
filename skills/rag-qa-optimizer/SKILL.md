---
name: rag-qa-optimizer
description: Use when designing or improving knowledge-base Q&A, retrieval, vector search, hybrid retrieval, grounded answers, or badcase feedback loops.
---

# 知识库问答 / RAG 优化

## 适用场景

Use when designing or improving knowledge-base Q&A, retrieval, vector search, hybrid retrieval, grounded answers, or badcase feedback loops.

## 使用方式

1. 先确认用户输入、资料范围、输出对象和禁止事项。
2. 优先遵循本仓库的长期协作偏好：中文、结构化、先结论、事实边界清楚、可直接复制使用。
3. 参考仓库中的 `templates/rag-qa-optimizer.md` 执行任务。
4. 输出时包含：结论 / 交付物 / 处理说明 / 待确认项 / 风险提示。
5. 收尾前执行 `checklists/sensitive-info-checklist.md`、`checklists/facts-boundary-checklist.md`，必要时执行 `checklists/task-closing-checklist.md`。

## 禁止事项

- 不输出账号、密码、token、cookie 或隐私信息。
- 不编造事实、数据、出处或政策依据。
- 不把一次性路径、临时判断、错误尝试沉淀为长期规则。
- 涉及外发、发送、线上写入或生产接口调用时，必须先获得用户确认。

## 输出模板

```text
## 结论摘要
## 处理过程 / 方法
## 结果 / 可复制内容
## 待确认项
## 风险提示
```
