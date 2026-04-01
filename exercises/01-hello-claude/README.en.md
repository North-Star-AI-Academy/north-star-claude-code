# Level 1: Hello Claude — Get Claude Code Up and Running

## Goal
Install Claude Code, understand how it works, and run your first commands.

## Exercises

### 1.1 — First interaction
Open this repo in your terminal and start Claude Code:
```bash
claude
```
Ask Claude: "What's in this repo?"

Claude automatically reads the `CLAUDE.md` file and understands the project structure.

### 1.2 — Discover slash commands
Try these commands:
- `/help` — View all available commands
- `/status` — Check the status of your session
- `/compact` — Compress your context (useful for long sessions)

### 1.3 — Reading and editing files
Ask Claude:
- "Read the README.md file and give me a summary"
- "Create a new file `my-notes.md` with 3 things I want to learn today"

### 1.4 — Understanding permission modes
Claude Code asks for permission before certain actions. You'll see this in the terminal:
- **Reading**: Always allowed
- **Writing**: Asks for permission (unless on the allowlist)
- **Bash commands**: Asks for permission

Tip: Press `y` to allow, `n` to deny.

## Checklist
- [ ] Claude Code is running
- [ ] You've asked a question and received an answer
- [ ] You've used a slash command
- [ ] You've had Claude create a file

## Done?
Move on to Level 2: `/start-exercise 2`
