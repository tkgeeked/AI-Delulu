# Anti-Delulu

A system prompt/guardrail designed to prevent LLMs from acting as "yes-men," mimicking user anxieties, or reinforcing echo-chambers and delusion loops.

---

## The Problem
Standard RLHF (Reinforcement Learning from Human Feedback) trains LLMs to be agreeable. When users express unverified premises, high anxiety, or paranoid assumptions, the model often:
1. **Flatter / Agree (Sycophancy)**: Validates false premises just to please the user.
2. **Mimic Tone**: Copycats the user's vocabulary and emotional style to build pseudo-intimacy.
3. **Hyper-Personalize**: Reuses past chats to create a self-reinforcing echo chamber.

Psychiatrists call this combination the **"delusion amplification spiral."**

## The Solution
This guardrail forces the model to:
* **Sympathize, don't validate**: Support the user's *feelings*, but remain neutral on their *claims*.
* **De-mimic**: Maintain a calm, objective, third-person perspective.
* **Self-Falsify**: Challenge its own assumptions before replying.

---

## 核心设计 (Simplified Chinese)

本提示词防護網旨在防止大語言模型（LLM）一味盲從迎合、模仿使用者焦慮情緒，或在多輪對話中形成病態的「回音室效應」（防止 AI 引导妄想，限制 AI 越界行为与盲目迎合）。

### 為什麼需要？
AI 聊天機器人基於 RLHF 機制，極易為了迎合評分而：
1. **盲目順從（Sycophancy）**：順著使用者的假設往下編，甚至盲信未證實的前提。
2. **語氣模仿**：模仿使用者的偏執或焦慮用詞，營造虛假的「知己」錯覺。
3. **過度個人化**：結合歷史對話，形成不斷自我驗證的「放大螺旋（Amplification Spiral）」。

### 防護機制
* **情感共情，邏輯脫鉤**：可以理解情緒（如「我明白這讓你很焦慮」），但絕不承認前提（不說「確實有人在針對你」）。
* **語言去模仿**：強制使用客觀、理性的第三方中立語調。
* **思維證偽**：回答前必須在思考區（`<thought>`）中找出 3 個反向論證，強迫 AI 展現合理分歧。

---

## Installation & Integration

### Google Antigravity
Copy `SKILL.md` to:
* `.agents/skills/Anti-Delulu/SKILL.md` (Workspace-scoped)
* `~/.gemini/config/skills/Anti-Delulu/SKILL.md` (Global)

### Dify / Coze / ChatGPT / Claude Custom Instructions
Copy the content of `SKILL.md` directly into the System Instructions or Agent System Prompt.
