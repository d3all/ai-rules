# Summary

- This file is a compact 40 lines global baseline for how Claude Code should write and modify code across projects, while project-level files handle stack-specific and architecture-specific rules. 
- ** Global or User-level CLAUDE.md ~/.claude **

# Purpose

- This Global CLAUDE.md defines a shared cross-project baseline for Claude’s coding behavior. It is meant to improve consistency, reduce overengineering, and make edits more predictable across different repositories.

# What It Covers

- It sets durable default rules for naming, structure, simplicity, dependencies, side effects, workflow, and comments. It does not define language-specific conventions, frameworks, or architecture patterns such as MVC, MVP, or MVVM, because those belong in project-level instructions.

# Why It Is Structured This Way

- The file is intentionally short, grouped into a few stable sections, and written as concrete behavioral rules rather than abstract slogans. This follows Anthropic’s guidance to use explicit, specific instructions for more reliable adherence and consistency.

# Relation to Anthropic Guidance

- This version aligns with Anthropic’s current recommendations by:
  - using direct, observable instructions instead of vague principles,
  - keeping persistent global rules focused on durable defaults,
  - leaving project-specific workflows, orchestration, and architecture to separate project-level files or routines.