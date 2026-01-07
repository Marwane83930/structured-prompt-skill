# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a prompt engineering reference library for building Claude skills. It contains curated AI system prompts from various tools and models, organized for easy reference when designing new prompts.

## Directory Structure

```
prompts/
├── awesome-gemini-prompts/     # Gemini prompts with Chinese role-play personas
│   └── prompts/                # 14 markdown files - learning frameworks, personas
├── GPTs/                       # 282 leaked GPT prompts from OpenAI GPT Store
│   └── prompts/                # Markdown files for each GPT
├── system-prompts-and-models-of-ai-tools/  # System prompts from 30+ AI tools
│   ├── Anthropic/              # Claude Code, Sonnet prompts
│   ├── Cursor Prompts/         # Cursor IDE prompts
│   ├── RooCode/, Codex CLI/, Gemini CLI/   # Open source tool prompts
│   └── [tool-name]/            # Each tool has its own directory
└── gpt-prompts/                # PROMPTS.md - ChatGPT role-play collection
```

## Prompt Format Patterns

Reference `prompts/awesome-gemini-prompts/prompts/` for well-structured Chinese prompts:
- Metadata header: needs, model, author, version
- Sections: 思维内核 (core thinking), 审美与禁忌 (aesthetics/taboos), 交互逻辑 (interaction logic), 初始化 (initialization)
- Use separator lines (━━━) and structured markdown

Reference `prompts/GPTs/prompts/` for GPT-style prompts:
- Command-based interaction (e.g., /test, /config, /plan)
- Knowledge file references
- Persona descriptions

## Claude Skill Development

When creating new skills for Claude:
1. Study existing patterns in `prompts/awesome-gemini-prompts/prompts/` for structured Chinese prompts
2. Use `prompts/system-prompts-and-models-of-ai-tools/Anthropic/` for Claude-specific patterns
3. Organize new prompts under appropriate subdirectories in `prompts/`

## Language Support

- English and Chinese prompts are both common
- For Chinese prompts, add: `使用简体中文回答，符合简体中文的表达习惯`
