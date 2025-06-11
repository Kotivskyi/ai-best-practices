# ai-best-practices
Collection of Best Practices for AI-driven software development workflow

## Project Structure

- Each best practice is a top-level folder in the repository (no nested `practices/` or `examples/` folders).
- Each practice folder must contain:
  - `README.md`: Overview, benefits, and when to use the practice.
  - `prompt.md`: Step-by-step guide or prompt for implementing the practice.
  - `example.*`: At least one code or markdown example (e.g., `example.js`, `example.md`).
- No `good/` or `bad/` subfolders; keep all files at the top level of each practice folder.
- All practice folders must be named using kebab-case (e.g., `clean-code`, `api-design`).

## Task List Management (from @task-list/task-list.mdc)

> **LOG:** This section is auto-synced with `task-list/task-list.mdc` for consistency. See that file for the canonical source.

### Task List Creation

1. Create task lists in a markdown file (in the project root):
   - Use `TASKS.md` or a descriptive name relevant to the feature (e.g., `ASSISTANT_CHAT.md`)
   - Include a clear title and description of the feature being implemented

2. Structure the file with these sections:

   ```markdown
   # Feature Name Implementation
   
   Brief description of the feature and its purpose.
   
   ## Completed Tasks
   
   - [x] Task 1 that has been completed
   - [x] Task 2 that has been completed
   
   ## In Progress Tasks
   
   - [ ] Task 3 currently being worked on
   - [ ] Task 4 to be completed soon
   
   ## Future Tasks
   
   - [ ] Task 5 planned for future implementation
   - [ ] Task 6 planned for future implementation
   
   ## Implementation Plan
   
   Detailed description of how the feature will be implemented.
   
   ### Relevant Files
   
   - path/to/file1.ts - Description of purpose
   - path/to/file2.ts - Description of purpose
   ```

### Task List Maintenance

1. Update the task list as you progress:
   - Mark tasks as completed by changing `[ ]` to `[x]`
   - Add new tasks as they are identified
   - Move tasks between sections as appropriate
2. Keep "Relevant Files" section updated with:
   - File paths that have been created or modified
   - Brief descriptions of each file's purpose
   - Status indicators (e.g., ✅) for completed components
3. Add implementation details:
   - Architecture decisions
   - Data flow descriptions
   - Technical components needed
   - Environment configuration

### AI Instructions

When working with task lists, the AI should:

1. Regularly update the task list file after implementing significant components
2. Mark completed tasks with [x] when finished
3. Add new tasks discovered during implementation
4. Maintain the "Relevant Files" section with accurate file paths and descriptions
5. Document implementation details, especially for complex features
6. When implementing tasks one by one, first check which task to implement next
7. After implementing a task, update the file to reflect progress

### Example Task Update

When updating a task from "In Progress" to "Completed":

```markdown
## In Progress Tasks

- [ ] Implement database schema
- [ ] Create API endpoints for data access

## Completed Tasks

- [x] Set up project structure
- [x] Configure environment variables
```

Should become:

```markdown
## In Progress Tasks

- [ ] Create API endpoints for data access

## Completed Tasks

- [x] Set up project structure
- [x] Configure environment variables
- [x] Implement database schema
```

## Maintenance Rules

- When adding, editing, or removing a practice, ensure the folder follows the structure above.
- When editing any project rule or changing the structure, you **must** update this `README.md` to reflect the latest rules and structure.
- Keep documentation clear and concise. Each file should be easy to read and understand.
- Use descriptive commit messages when making changes to practices or project rules.
- Review and refactor existing practices periodically to ensure consistency and quality.

## Contribution Guidelines

- All contributions must follow the structure and maintenance rules above.
- Pull requests should include updates to `README.md` if any rule or structure is changed.
- New practices should be reviewed for clarity, accuracy, and adherence to the structure before merging.

---

**Remember:**
- The main `README.md` is the source of truth for the project structure and rules. Always keep it up to date!

## Contents

- [task-list.mdc](task-list/task-list.mdc): Guidelines and best practices for creating, maintaining, and updating task lists using markdown and AI. Includes instructions for structuring tasks, updating progress, and leveraging AI for task management.

## Description of Items

### task-list.mdc
This document describes how to create and manage task lists using markdown files It covers:
- How to structure task lists for features and projects
- Best practices for updating and maintaining task lists
- How AI should interact with and update task lists
- Example formats for completed, in-progress, and future tasks


### EXAMPLE_TASK.md
This file showcases how to create and manage a task list for a feature, following the guidelines in task-list.mdc. It includes:
- Example sections for completed, in-progress, and future tasks
- An implementation plan
- A relevant files list
- Realistic example items to illustrate proper usage
