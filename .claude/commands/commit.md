# Create a Commit

Create a git commit for the current staged and unstaged changes.

## Tasks

1. **Check current state**:
   - Run `git status` to see all untracked and modified files
   - Run `git diff` to see unstaged changes
   - Run `git diff --staged` to see staged changes
   - Run `git log --oneline -5` to see recent commit message style

2. **Analyze changes**:
   - Review all changes that will be committed
   - Categorize the change type (feature, fix, refactor, docs, chore, etc.)
   - Do NOT commit files that may contain secrets (.env, credentials, etc.)

3. **Stage and commit**:
   - Stage relevant files with `git add`
   - Write a concise commit message that focuses on the "why" rather than the "what"
   - Use conventional commit format: `type: description`
   - End the commit message with:

4. **Verify**:
   - Run `git status` after commit to verify success
   - If pre-commit hooks modify files, amend the commit (only if you authored it)

## Rules

- NEVER push to remote unless explicitly asked
- NEVER use `--force` or destructive git commands
- NEVER skip hooks (`--no-verify`)
- NEVER amend commits you didn't author
- If there are no changes, do not create an empty commit
