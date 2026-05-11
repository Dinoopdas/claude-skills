# 🧠 Claude Custom Skills

A collection of custom skills for [Claude](https://claude.ai) that enhance productivity, reduce token usage, and optimize workflows.

## What Are Skills?

Skills are instruction sets that change how Claude behaves for specific tasks. They're like plugins — drop one into a conversation and Claude adapts its approach accordingly. Skills persist across messages within a session and can be combined for compounding effects.

## 📦 Available Skills

### Lean Mode

> **File:** `lean-mode.skill`
> **Token savings:** 40–60% across all task types

An operational efficiency mode that reduces context window consumption by changing *how Claude works* — not just how it talks. Covers text responses, code generation, PDF creation, PDF analysis, file processing, and tool usage.

**What it does:**

| Area | Strategy | Savings |
|------|----------|---------|
| Text | Eliminates preambles, recaps, unnecessary caveats | ~50% |
| Code | Compact idioms, surgical edits over full rewrites | ~35–70% |
| PDF creation | Single-script, inline content, direct-to-output | ~45% |
| PDF analysis | Triage-first, targeted page extraction | ~60% |
| Tool calls | Batched commands, `view_range`, suppressed verbose output | ~40–50% |

**Activation commands:**

```
/lean
lean mode
save tokens
efficient mode
```

**Deactivation:**

```
normal mode
stop lean
```

**Stacks with:** Caveman mode (lean = operational efficiency, caveman = prose compression). Together they achieve 70–80% token reduction.

## 🔧 Installation

1. Download the `.skill` file from this repo
2. Open a conversation on [claude.ai](https://claude.ai)
3. Drag and drop the `.skill` file into the chat
4. Claude confirms installation — the skill is now active for all your conversations

Alternatively, upload the `.skill` file using the attachment button (📎) in any chat.

## 💡 Usage Tips

- Lean mode is most impactful in **long sessions** where context builds up — technical projects, multi-file processing, iterative code editing
- Activate early in a conversation for maximum savings
- Combine with the `/token-status` command to monitor consumption in real time
- The skill auto-intensifies when context usage exceeds 60%

## 🗂️ Repo Structure

```
claude-skills/
├── README.md
└── lean-mode.skill
```

## 📝 License

MIT — use, modify, and share freely.

## 👤 Author

**Dinoop Das**
GitHub: [@Dinoopdas](https://github.com/Dinoopdas)
