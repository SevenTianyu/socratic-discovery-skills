# Socratic Discovery Skills

[简体中文](./README.zh-CN.md)

Socratic Discovery is a pair of language-specific skills for guided Socratic exploration. Instead of rushing to provide answers, these skills help an assistant ask one thoughtful question at a time so the user can build understanding through their own reasoning.

This repository includes:

- `socratic-discovery-en`: English-first version
- `socratic-discovery-zh`: Chinese-first version

Both versions are designed to help users explore:

- confusion that is still hard to name clearly
- blind spots and hidden assumptions
- "unknown unknowns"
- deeper understanding through self-generated thinking

## Who This Is For

These skills are intended for assistant workflows such as Codex and Claude Code when you want a more question-led mode of thinking. They are especially useful when the user:

- wants to unpack a vague or difficult topic
- prefers guided thinking over direct explanation
- wants to think more independently instead of being handed a conclusion
- is working through technical, strategic, reflective, or open-ended questions

## What Each Skill Does

Each skill turns the assistant into a patient Socratic guide that:

- starts by collecting the user's current baseline
- asks one real question at a time
- adjusts difficulty based on the user's answers
- notices thought patterns and blind spots
- closes by asking the user to restate what they now understand

## Choose a Version

Use [socratic-discovery-en/SKILL.md](./socratic-discovery-en/SKILL.md) if you want the interaction to default to English.

Use [socratic-discovery-zh/SKILL.md](./socratic-discovery-zh/SKILL.md) if you want the interaction to default to Chinese.

## Install from This Repository

1. Open this repository in your browser, or clone it locally.
2. Pick the skill folder you want to use:
   `socratic-discovery-en` or `socratic-discovery-zh`
3. Copy that folder into the local skills library used by your assistant setup.
4. Reload or restart the assistant if your environment does not auto-refresh local skills.

You can also keep both folders and choose the language at invocation time.

## Use with Codex

Once the chosen skill folder is available in your local skills library, invoke it by name:

- `Use $socratic-discovery-en to help me think through something I do not understand yet by asking one question at a time.`
- `Use $socratic-discovery-zh to guide me in Chinese through a topic I do not fully understand yet, one question at a time.`

## Use with Claude Code

If your Claude Code workflow supports reusable local skills or similar prompt-pack folders, add the chosen skill folder to that library and invoke it by folder name in the same way:

- `Use $socratic-discovery-en ...`
- `Use $socratic-discovery-zh ...`

The important part is not a fixed path. What matters is that the selected skill folder is available to your assistant as a local reusable skill.

## Repository Layout

- [socratic-discovery-en/SKILL.md](./socratic-discovery-en/SKILL.md)
- [socratic-discovery-en/agents/openai.yaml](./socratic-discovery-en/agents/openai.yaml)
- [socratic-discovery-zh/SKILL.md](./socratic-discovery-zh/SKILL.md)
- [socratic-discovery-zh/agents/openai.yaml](./socratic-discovery-zh/agents/openai.yaml)
