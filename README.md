# Reexplain For Me

A Codex skill for adults who know the basics of a field and want help understanding a specialist concept. It starts from what you already know and breaks the difficult part into steps you can follow.

## How to use it

Invoke `$reexplain-for-me` in your prompt. Say what you already understand and point to the part that lost you. If you're working from a passage, diagram, or error message, include the relevant excerpt.

```text
Use $reexplain-for-me. I know what a database index does.
Walk me through why a query planner might scan the whole table anyway.
Use one example and carry it through each step.
```

If one step still feels unclear, ask about that step directly. For example, “Go back to the step about the cost of looking up matching rows. Show it with a smaller example.”

## What to expect

- A short answer first, followed by one new idea at a time. Specialist terms are defined when they come up, and missing prerequisites are explained where they are needed.
- One example carried through the steps when it helps. If the skill uses an analogy, it explains where the analogy stops matching the real concept when that matters.
- Confidence labels for groups of related claims. `[Certain]` signals direct evidence, `[Likely]` signals a strong inference, and `[Guessing]` signals a gap in the evidence. Important assumptions and uncertain conclusions get their own labels.
- A comparison when you face a choice. The skill explains where each option fits and which benefits, risks, or requirements affect your decision.

The full instructions are in [SKILL.md](SKILL.md). The display name and default prompt are in [agents/openai.yaml](agents/openai.yaml).
