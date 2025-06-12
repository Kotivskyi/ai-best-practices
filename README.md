# AI Best Practices

A comprehensive collection of best practices, templates, and guidelines for AI-driven software development workflows. This repository provides practical frameworks for enhancing productivity and code quality when working with AI coding assistants like GitHub Copilot, Cursor, and Claude.

## What's Inside

This repository contains proven practices for:
- **Task Management**: Structured approaches to planning and tracking development work with AI assistance
- **Custom Instructions**: Templates and examples for configuring AI assistants to understand your project context
- **Planning Frameworks**: Methodologies for breaking down complex features and managing AI-assisted development workflows
- **Development Best Practices**: Guidelines for effective human-AI collaboration in software development

## Repository Structure

```
ai-best-practices/
├── custom-instructions/     # Templates and examples for AI assistant configuration
│   └── copilot-instructions.md
├── planning/               # Project planning methodologies and templates
│   ├── create-plan.prompt.md
│   └── task-maintenance.instructions.md
├── task-list/             # Task management frameworks and examples
│   ├── task-list.mdc
│   └── TASK.example.md
└── README.md              # This file - project overview and guidelines
```


## Custom Instructions for AI Assistants

By adding custom instructions to your repository, you can guide Copilot on how to understand your project and how to build, test and validate its changes.

If Copilot is able to build, test and validate its changes in its own development environment, it is more likely to produce good pull requests which can be merged quickly.

Add instructions to a .github/copilot-instructions.md file in the repository. For more information, see Adding repository custom instructions for GitHub Copilot.

Here is an example of effective instructions: [copilot-instructions.md](custom-instructions/copilot-instructions.md)

### Task Maintenance Instructions

The [task-maintenance.instructions.md](planning/task-maintenance.instructions.md) file provides specific guidance for AI assistants on how to maintain and update task lists during development. This ensures that:

- Task progress is consistently tracked and updated
- Implementation details are documented as they're discovered
- File references remain accurate throughout development
- AI assistants follow structured approaches to task management

These instructions are designed to work with task files that follow the `*TASK*.md` naming pattern.

## Planning Framework

The [create-plan.prompt.md](planning/create-plan.prompt.md) provides a structured template for creating development plans with AI assistance. This template:

- Guides AI assistants to search the codebase before creating plans
- Focuses on planning rather than immediate implementation
- Creates structured task lists for tracking progress
- Includes guidance for manual testing workflows
- Ensures clear documentation of implementation details

Use this template when starting new features or complex changes to get well-structured, actionable development plans.


## Project Maintenance Rules

- When adding, editing, or removing a practice, ensure it follows the repository structure defined above
- When editing any project rule or changing the structure, you **must** update this `README.md` to reflect the latest changes
- Keep documentation clear and concise - each file should be easy to read and understand  
- Use descriptive commit messages when making changes to practices or project rules
- Review and refactor existing practices periodically to ensure consistency and quality
- Test any custom instructions or templates before including them in the repository

## Contributing

We welcome contributions to improve and expand these AI development best practices!

### Contribution Guidelines

- All contributions must follow the repository structure and maintenance rules above
- Pull requests should include updates to `README.md` if any structure or rules are changed
- New practices should be reviewed for clarity, accuracy, and practical applicability
- Include examples or templates when introducing new methodologies
- Ensure all documentation is beginner-friendly and well-explained

### Before Contributing

1. Check existing practices to avoid duplication
2. Test your approach in a real project context
3. Follow the established documentation format
4. Include clear examples and use cases

---

**Remember:**
- The main `README.md` is the source of truth for the project structure and rules. Always keep it up to date!


## References

- **Realworld Project Rules Example:** 
  [elie222/inbox-zero – .cursor/rules](https://github.com/elie222/inbox-zero/tree/main/.cursor/rules)

- **Cursor Guides:**  
   [Advanced: Large Codebases](https://docs.cursor.com/guides/advanced/large-codebases)

- **Claude Code Best Practices:**  
   [Claude Code Best Practices](https://www.anthropic.com/engineering/claude-code-best-practices)

- **GitHub Copilot Guides:**  
   [GitHub Copilot Documentation](https://docs.github.com/en/copilot/using-github-copilot)

- **VS Code GitHub Copilot Guides:**  
   [Copilot Customization in VS Code](https://code.visualstudio.com/docs/copilot/copilot-customization)