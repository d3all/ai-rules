# Global User-level CLAUDE.md ~/.claude

## Naming & Structure
- Make code understandable from names and structure before relying on comments.
- Use meaningful, descriptive names for variables, functions, types, and modules.
- Keep file structure, naming, and APIs consistent and predictable.
- Keep functions small enough that their purpose is obvious from the code shape.
- Avoid cryptic shortcuts, unclear flags, and overloaded function behavior.
- One module, class, or function should solve one clear task.
- When adding new behavior, prefer a new scoped component over rewriting unrelated existing logic.

## Simplicity & Maintainability
- Prefer the simplest solution that correctly solves the problem and remains easy to modify and debug.
- Eliminate redundant code.
- Do not add speculative abstractions or code unless they are needed for the current task or explicitly requested.
- Avoid abstractions that make routine changes harder.
- Prefer readable code by default; optimize only when the change is justified by a measured or likely bottleneck.

## Dependencies & Side Effects
- Prefer minimal and explicit dependencies; avoid unnecessary libraries.
- Pass dependencies explicitly; avoid hard-wiring concrete implementations inside business logic.
- Avoid hidden side effects; keep functions predictable and explicit.
- Validate inputs early when invalid data can break the flow.
- Handle non-trivial errors explicitly.
- Do not change expected input/output behavior in replacements of the same contract.

## Behavior & Workflow
- If modifying existing code, follow existing patterns and structure.
- If requirements are unclear, ask for clarification instead of guessing.
- If logic is non-trivial or critical, write unit tests.

## Writing Style & Comment Rules
- Use clear, concise language.
- Use English only for code, comments, and error messages.
- Write descriptive comments only where they add useful context.
- Each meaningful block, should explain:
  - what is happening
  - why this step is needed
- Do not comment trivial or obvious lines.
- Keep comments short and meaningful.
- Do not just restate the code or repeat function names.

## Execution Discipline
- State assumptions explicitly when they affect the implementation.
- Touch only code that is directly related to the task.
- Before finishing a non-trivial change, run or describe a concrete verification step that confirms the result.
- Stop when the task is done. Do not continue with adjacent improvements unless asked.