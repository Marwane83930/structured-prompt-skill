# Contributing Guide

Thank you for your interest in contributing to the Structured Prompt Writer project!

## How to Contribute

### Adding New Prompts

1. **Fork the repository**
2. **Choose the appropriate directory**:
   - `skills/structured-prompt-writer/references/prompts/personas/` - For persona-based prompts
   - `skills/structured-prompt-writer/references/prompts/creative/` - For creative/writing prompts
   - `skills/structured-prompt-writer/references/prompts/system-tools/` - For AI tool system prompts
   - `skills/structured-prompt-writer/references/prompts/gpts-personas/` - For GPT-style prompts

3. **Follow the naming convention**:
   - Use descriptive names: `ProductManager.md`, `TechWriter.md`
   - For Chinese prompts: `产品经理.md`, `技术写作.md`

4. **Use the appropriate format**:

   For structured prompts:
   ```markdown
   ---
   needs: [list of requirements]
   model: [recommended model]
   author: your-name
   version: 1.0
   ---

   # Prompt Title

   ## Description
   [Brief description of the prompt's purpose]

   ## Prompt Content
   [The actual prompt]
   ```

   For system prompts:
   ```markdown
   # Tool Name - Prompt Type

   Source: [URL or reference]
   Date: YYYY-MM-DD

   ---

   [Prompt content]
   ```

5. **Submit a Pull Request**

### Improving Existing Prompts

- Fix typos or grammatical errors
- Improve clarity and structure
- Add missing metadata
- Update outdated information

### Reporting Issues

Please include:
- Description of the issue
- Steps to reproduce (if applicable)
- Expected vs actual behavior
- Screenshots (if helpful)

## Code of Conduct

- Be respectful and inclusive
- Provide constructive feedback
- Focus on improving the project

## Style Guidelines

### Markdown
- Use proper heading hierarchy (H1 > H2 > H3)
- Include blank lines between sections
- Use code blocks for prompt content

### Prompt Quality
- Clear and unambiguous instructions
- Appropriate context and constraints
- Well-defined output format
- Tested with target models

### Language
- English for documentation
- Prompts can be in any language
- Add language tags when not English

## Questions?

Open an issue with the `question` label or start a discussion.
