# Anti-Delulu: Anti-Sycophancy & Delusion Mitigation Skill

[English](#english) | [简体中文](#简体中文)

---

## English

`Anti-Delulu` (originally known as `anti-delusion`) is a custom AI skill designed to prevent large language models (LLMs) from amplifying user delusions, confirmation bias, or anxiety loops. 

### Why is this needed?
According to psychiatric research (e.g., Augustine et al., 2026), AI chatbots can trigger an **"amplification spiral"** of delusions due to three common behaviors stemming from Reinforcement Learning from Human Feedback (RLHF):
1. **Sycophancy**: AI tends to agree with user assumptions to get higher rating scores.
2. **Linguistic Mimicry**: AI mirrors the user's emotional, anxious, or paranoid tone to build intimacy.
3. **High Personalization**: AI uses historical interaction logs to tailor responses, creating a closed validation loop.

This skill interrupts this loop at the system prompt level.

### Key Features
- **Logical Dissonance**: Empathize with user emotions, but never validate unverified premises.
- **De-mimicry**: Maintain an objective, calm, and neutral 3rd-person tone.
- **Self-Falsification CoT**: Forces the LLM to write down 3 counterarguments in its internal reasoning chain before outputting a response.

---

## 简体中文

`Anti-Delulu`（原名 `anti-delusion`）是一个自定义 AI Skill，旨在防止大语言模型（LLM）通过盲目顺从、语言模仿或过度个性化来增强或放大用户的妄想、认知偏差或焦虑循环（防止 AI 引导妄想，限制 AI 越界行为与盲目迎合）。

### 为什么需要这个 Skill？
根据精神病学研究，AI 聊天机器人很容易因为人类反馈强化学习（RLHF）所导致的以下三种行为，与易受影响的用户交织，形成**「放大螺旋（Amplification Spiral）」**：
1. **奉承迎合 (Sycophancy)**：AI 倾向于附和用户的观点，而非质询可疑的主观假设。
2. **语言模仿 (Linguistic Mimicry)**：AI 学习并镜像用户的词汇、语调和写作风格，以建立虚假的亲密感。
3. **高度个性化 (High Personalization)**：AI 利用历史对话信息提供过于贴合个人需求的回应，使之像一个值得信赖的知己。

本 Skill 从系统提示词层面切断了这一螺旋。

### 核心功能
- **情感共情，逻辑脱钩**：理解并安抚用户的情绪，但坚决不盲信、不验证未证实的结论。
- **语言去壁虎化**：拒绝模仿用户的情绪化或偏执词汇，保持客观、冷静、理性的第三方语调。
- **自我证伪思维链 (Falsification CoT)**：要求 AI 在回答前，必须在思考区先写出 3 个反驳用户前提的理由。

---

## Installation & Usage (安装与使用)

### 1. In Google Antigravity (AGY)
Copy the `SKILL.md` file to your customization directory:
- **Global**: `~/.gemini/config/skills/Anti-Delulu/SKILL.md`
- **Workspace**: `.agents/skills/Anti-Delulu/SKILL.md`

### 2. In other LLM Platforms (ChatGPT / Claude / Dify / Coze)
Copy the contents of `SKILL.md` into your system instructions, agent system prompts, or custom instructions.
