# Level 6: Git Workflows — Version control with Claude

## Goal
Learn how Claude Code works with Git for version control, branches, and worktrees.

## Theory

Claude Code understands Git natively. It can:
- Create commits with clear messages
- Create and manage branches
- Resolve merge conflicts
- Use Git worktrees for parallel features

## Exercises

### 6.1 — Your first commit with Claude
Make a change and let Claude commit it:

```
Add a file: my-marketing-plan.md with a short description
of 3 marketing goals for Q2 2026. Commit this with a clear message.
```

Notice: Claude writes a descriptive commit message and only stages relevant files.

### 6.2 — Branching
```
Create a new branch "feature/linkedin-strategy" and add a file
linkedin-plan.md with a 4-week content plan. Commit on that branch.
```

### 6.3 — Git worktrees (advanced)
Worktrees let you work on multiple branches at the same time, each in its own directory:

```
Explain what git worktrees are and when I would use them.
Give a practical example for a marketer who is working on
a blog post and an email campaign at the same time.
```

### 6.4 — Viewing commit history
```
Look at the git log of this project and give me a summary
of the last 5 commits.
```

### 6.5 — Good commit messages
Claude writes good commits by default, but you can guide it:

```
Make a change to README.md (add a "My Notes" section)
and commit with a conventional commit message (feat:, fix:, docs:, etc.)
```

## Tips
- Claude always asks for permission before committing or pushing
- Claude NEVER pushes to remote automatically — you have to explicitly ask
- Use branches for experiments, merge to main when you're happy with the result

## Checklist
- [ ] You've made a commit via Claude
- [ ] You've created a branch
- [ ] You understand what worktrees are
- [ ] You can view git history via Claude

## Done?
Move on to Level 7: `/start-exercise 7`
