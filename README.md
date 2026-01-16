# Agent-Skills
Save useful skills
# Agent Skills Handbook

> This document is the **English version of the Agent Skills handbook**, suitable for global teams and open-source sharing.

---

## 1. What is an Agent Skill

An **Agent Skill** is a reusable, modular capability that equips an AI agent with a specific expertise.

A skill typically lives in its own folder and is centered around a `SKILL.md` file that defines:

* What the skill does
* When it should be used
* How the agent should act
* How results should be presented

---

## 2. How to Use Agent Skills

### 2.1 User Perspective

**Steps:**

1. Place the skill folder under the `skills/` directory
2. Describe your task in natural language
3. The agent automatically selects relevant skills
4. The skill guides execution and output

You usually **do not need to explicitly mention the skill name**.

---

### 2.2 Skill Author Perspective

A good skill clearly defines:

* When to use it
* Step-by-step instructions
* A predictable output format

---

## 3. Role-based Skill Sets

### Frontend Engineer

* code-review
* bug-triage
* doc-coauthoring
* workflow-orchestrator

### Tech Lead

* research-assistant
* workflow-orchestrator
* doc-coauthoring

### Product Manager

* research-assistant
* doc-coauthoring
* data-analysis

---

## 4. Example SKILL.md (Ready to Use)

### 4.1 code-review

```md
---
name: code-review
description: Review code for quality, maintainability, and potential issues
version: 1.0
---

## When to use
Use this skill when the user provides code and asks for review or improvement.

## Instructions
1. Understand the code context
2. Review readability, naming, and structure
3. Identify bugs or performance risks
4. Provide actionable improvement suggestions

## Output format
- Overall assessment
- Issues
- Recommendations
```

---

### 4.2 bug-triage

```md
---
name: bug-triage
description: Analyze bug reports and determine root cause and priority
version: 1.0
---

## When to use
Use this skill when the user reports a bug or unexpected behavior.

## Instructions
1. Understand the issue description
2. Infer possible root causes
3. Assess impact and priority
4. Suggest fixes or investigation steps

## Output format
- Bug summary
- Possible causes
- Priority
- Suggested actions
```

---

## 5. Resources

* Skill0 Marketplace: [https://skill0.atypica.ai/](https://skill0.atypica.ai/)
* Agent Skills Specification: [https://agentskills.io/specification](https://agentskills.io/specification)
