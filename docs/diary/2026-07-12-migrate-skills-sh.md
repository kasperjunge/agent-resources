# Diary: Migrate agr repository skills to skills.sh

Move the repository's own agent skills off its legacy self-hosted configuration.

## Step 1: Convert active skills

**Author:** main

### Prompt Context
**Verbatim prompt:** you should also do it for the other projects and repos.
**Interpretation:** Include the agr repository in the cross-repo migration.
**Inferred intent:** Stop relying on agr even for agr's development workspace.

### What I did
Installed `agr-release`, `code-review`, and `playwright-cli` for Claude Code and Codex, created `/skills-lock.json`, removed `/agr.toml` and `/agr.lock`, and removed the public README warning at the user's request.

### Why
The repository should use the same active skill manager as the other workspaces without publicly declaring the project unmaintained.

### What worked
The three available skills validated and installed successfully.

### What didn't work
`github-issue-triage` was no longer present in `computerlovetech/skills`. Remote ralph dependencies are not supported by skills.sh.

### What I learned
Several legacy manifest entries no longer resolve to published resources.

### What was tricky
The migration and the explicit reversal of the README notice needed to land together without rewriting product documentation about agr itself.

### What warrants review
Review `/skills-lock.json`, the README warning removal, and the omitted stale/ralph dependencies.

### Future work
Decide separately whether any remote ralph dependencies still need another installation mechanism.
