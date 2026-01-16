# Agent Skills 使用手册（中文版）

> 本文档为 **Agent Skills 中文版完整手册**，用于团队内部使用、学习与落地。

---

## 1. 什么是 Agent Skill

Agent Skill（智能体技能）是一种 **可复用、模块化的能力单元**，用于为 AI Agent 提供某一类明确、稳定的专业能力。

一个 Skill 通常以文件夹形式存在，核心是 `SKILL.md` 文件，用于告诉 Agent：

* 这个技能解决什么问题
* 什么时候应该使用
* 应该如何执行
* 最终如何输出结果

---

## 2. Agent Skills 的使用方法

### 2.1 使用者视角

**步骤：**

1. 将 Skill 文件夹放入 `skills/` 目录
2. 用自然语言描述你的任务
3. Agent 自动判断并加载 Skill
4. Skill 指导 Agent 执行并输出结果

你通常 **不需要显式点名 Skill**。

---

### 2.2 Skill 作者视角

一个高质量 Skill 应该包含：

* 明确的使用时机（When to use）
* 清晰的执行步骤（Instructions）
* 稳定的输出格式（Output format）

---

## 3. 按角色推荐的 Skills 组合

### 前端工程师

* code-review
* bug-triage
* doc-coauthoring
* workflow-orchestrator

### 技术负责人

* research-assistant
* workflow-orchestrator
* doc-coauthoring

### 产品经理

* research-assistant
* doc-coauthoring
* data-analysis

---

## 4. 示例 SKILL.md（可直接使用）

### 4.1 code-review

```md
---
name: code-review
description: 对代码进行质量、可维护性和潜在问题审查
version: 1.0
---

## When to use
当用户提供代码，并希望获得改进建议、风险提示或最佳实践时使用。

## Instructions
1. 阅读代码并理解上下文
2. 检查可读性、命名、结构
3. 指出潜在 Bug 和性能问题
4. 给出具体、可执行的改进建议

## Output format
- 总体评价
- 问题列表
- 改进建议
```

---

### 4.2 bug-triage

```md
---
name: bug-triage
description: 分析 Bug 描述并判断原因与优先级
version: 1.0
---

## When to use
当用户描述 Bug、异常行为或线上问题时使用。

## Instructions
1. 理解 Bug 现象
2. 推测可能原因
3. 判断影响范围与优先级
4. 提出修复或排查建议

## Output format
- Bug 摘要
- 可能原因
- 优先级
- 建议方案
```

---

## 5. 资源

* Skill0 Marketplace: [https://skill0.atypica.ai/](https://skill0.atypica.ai/)
* Agent Skills Spec: [https://agentskills.io/specification](https://agentskills.io/specification)
