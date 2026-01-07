# GEMINI.md

This file provides context for the Gemini AI agent working within this repository.

## Project Overview

This is a **Prompt Engineering Reference Library** and **AI Skill Repository**. It serves as a comprehensive knowledge base for building, analyzing, and refining AI system prompts, personas, and agentic skills. It aggregates resources from various ecosystems (Gemini, OpenAI/GPT, Anthropic/Claude) and open-source AI tools.

## Directory Structure

### `prompts/`
The core knowledge base, categorized by source and model type:

*   **`gemini-structured/`**: A collection of high-quality prompts specifically optimized for Gemini (formerly `awesome-gemini-prompts`).
    *   **Focus:** Chinese role-play personas, structured thinking frameworks (e.g., "Think微调版", "PDCA-ASK").
    *   **Best Practices:** Reference this directory for examples of complex, structured markdown prompts.
*   **`gpts-personas/`**: Contains "leaked" or reverse-engineered system prompts from the OpenAI GPT Store (formerly `GPTs`).
    *   **Use Case:** Analyzing how specialized "GPTs" are constructed (instruction sets, knowledge retrieval).
*   **`system-tools/`**: A vast collection of system prompts used by commercial AI tools and IDEs (formerly `system-prompts-and-models-of-ai-tools`).
    *   **Includes:** Anthropic (Claude), Cursor, GitHub Copilot, and various coding assistants.
    *   **Value:** Understanding how production-grade AI tools are instructed to behave.
*   **`collections/`**: General prompt lists and collections.
    *   **Includes:** `awesome-chatgpt-prompts.md` (formerly `gpt-prompts/PROMPTS.md`).
*   **`resources/`**: Documentation, guides, and PDFs (e.g., Gemini Prompting Guide 101).

### `skills/`
Contains definition files for specific "skills" that can be loaded or referenced by AI agents.

*   **`structured-prompt-writer/`**: A specialized skill designed to help users write professional, structured AI prompts.
    *   **`SKILL.md`**: Documentation for this skill, explaining its modes (Detailed vs. Simple) and the "LangGPT" structured format it employs.

### Root Files
*   **`CLAUDE.md`**: Provides specific guidance for Claude Code, outlining the prompt formats and directory organization. Useful as a general reference for repository conventions.
*   **`structured-prompt-writer.skill`**: The binary or configuration file defining the structured prompt writing skill.

## Key Concepts & Conventions

### Structured Prompting (LangGPT Style)
The repository heavily favors "Structured Prompts" (often associated with the LangGPT methodology). Key characteristics observed in `awesome-gemini-prompts`:
*   **Metadata Headers:** `Name`, `Author`, `Version`, `Model`.
*   **Markdown Structure:** Use of extensive Markdown for hierarchy (`#`, `##`, `###`), separators (`━━━`), and lists.
*   **Role Definition:** Clearly defined `## Profile`, `## Skills`, `## Rules` (Constraints/Taboos), and `## Workflow`.
*   **Initialization:** A distinct `## Initialization` section where the AI sets up its persona.

### Usage Guide for Gemini

1.  **Prompt Research:** Search the `prompts/` directory to find examples of specific personas (e.g., "Coder", "Academic Writer", "Debater") to understand effective instruction patterns.
2.  **Skill Application:** If asked to write a prompt, adopt the persona of the **Structured Prompt Writer** (defined in `skills/structured-prompt-writer/SKILL.md`).
    *   Follow the "Detailed Mode" or "Simple Mode" workflows.
    *   Ensure generated prompts include clear headers, constraints, and initialization steps.
3.  **Language:** Be aware that a significant portion of the high-quality structured prompts in `awesome-gemini-prompts` are in **Chinese**. When analyzing or generating prompts for Chinese users, adhere to the "Simplified Chinese" conventions found there.

## Development Tasks

If asked to maintain or expand this repository:
*   **New Prompts:** Place them in the appropriate subdirectory based on the target model.
*   **Format:** Adhere to the structured Markdown format found in `awesome-gemini-prompts` for consistency.
*   **Documentation:** Update `README.md` files in subdirectories if new categories are added.
