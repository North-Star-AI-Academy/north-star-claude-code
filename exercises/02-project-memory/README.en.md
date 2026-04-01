# Level 2: Project Memory — Help Claude Remember Your Project

## Goal
Understand how CLAUDE.md works and why it's essential. Without CLAUDE.md, Claude wastes up to 33,000 tokens "figuring out" your project — every single time.

## Theory

Claude Code automatically reads these files:
1. **`CLAUDE.md`** in your project root — project rules and context
2. **`~/.claude/CLAUDE.md`** — personal rules (across all your projects)
3. **`.claude/settings.json`** — technical settings

## Exercises

### 2.1 — Analyze the existing CLAUDE.md
Ask Claude: "Analyze this project's CLAUDE.md file. What's in it and why?"

### 2.2 — Write your own CLAUDE.md
Create a new project (simulation) and write a CLAUDE.md for it:

```
Create a folder `my-marketing-project/` with a CLAUDE.md file for a
fictional marketing agency. The agency is called "Bright Spark" and specializes
in B2B SaaS marketing. They use HubSpot, Figma, and write content in
Dutch.
```

A good CLAUDE.md includes:
- What the project is (1-2 sentences)
- Tech stack / tools
- Conventions (language, tone of voice, naming)
- Key files and folder structure
- What Claude should and shouldn't do

### 2.3 — Set up global rules
Create a personal rules file:

```
Create a file ~/.claude/CLAUDE.md with my personal preferences:
- I'm a marketer, not a developer
- Always respond in English unless I ask for another language
- Keep explanations simple and practical
- Don't use technical jargon without explaining it
```

### 2.4 — Set up Product Context
Use the product-context skill:
```
/product-context
```
Fill in the questions for your own company or a fictional one. This file is automatically used by all marketing skills.

## Checklist
- [ ] You understand what CLAUDE.md does
- [ ] You've written your own CLAUDE.md
- [ ] You've set up global rules
- [ ] You've created a product-context.md

## Done?
Move on to Level 3: `/start-exercise 3`
