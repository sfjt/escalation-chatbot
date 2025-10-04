# Escalation Chatbot Prompts

A comprehensive set of prompts and knowledge files designed to help technical support engineers write effective escalation tickets that get faster reaction/resolution from development and engineering teams.

**Note:** The instructions are intentionally designed to be restrictive for educational purposes so the user can learn best practices through chatting.

## Initial Setup

1. Rename `config.md.example` to `config.md` and update it:
   - **Company Context**: Replace `N/A` in the section with your actual company or product name (e.g., `Company or product name: Acme Corporation`). This enables the AI agent to reference your official documentation when encountering unfamiliar product features.
   - **Domain Access Control**: Add domain names that AI agents may not search or fetch. These prohibited domain names are typically for your company's internal inspection, logging, or ticketing tools. 
2. Deploy the set of prompts as a [Gem](https://support.google.com/gemini/answer/15236405) or a [GPT](https://openai.com/index/introducing-gpts/).

## Core Files

| File | Purpose |
|------|---------|
| `prompts/instructions.md` | Main workflow with investigation guidance |
| `prompts/knowledge/best_practices.md` | Comprehensive escalation writing guidelines |
| `prompts/knowledge/priorities.md` | Priority definitions with clear decision framework |
| `prompts/knowledge/good_examples.md` | Effective escalation examples to model |
| `prompts/knowledge/bad_examples.md` | Learning examples with improvement guidance |
| `prompts/knowledge/config.md` | Agent configuration |
