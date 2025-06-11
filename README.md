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
│   └── plan.mdc
├── task-list/             # Task management frameworks and examples
│   ├── task-list.mdc
│   └── TASK.example.md
└── README.md              # This file - project overview and guidelines
```

## Getting Started

1. **Browse the practices**: Start with the folder that matches your current need
2. **Adapt to your project**: Copy and modify templates to fit your specific requirements
3. **Configure your AI**: Use the custom instructions to improve AI assistant performance
4. **Follow the workflow**: Implement the task management and planning practices in your development process

## Planning for AI-Assisted Development

For larger changes, spending an above-average amount of thought to create a precise, well-scoped plan can significantly improve AI assistant output quality and reduce iteration cycles.

### When to Create a Detailed Plan

If you find that you're not getting the result you want after a few different variations of the same prompt, consider zooming out and creating a more detailed plan from scratch, as if you were creating a PRD (Product Requirements Document) for a coworker. 

**Key insight**: Oftentimes the hard part is figuring out *what* change should be made—a task suited well for humans. With the right instructions, we can delegate parts of the *implementation* to AI assistants.

### Using AI to Augment Plan Creation

One effective approach is to use your AI assistant's conversation mode to help create the plan itself:

1. **Gather context**: Collect information from your project management systems, internal docs, or loose thoughts
2. **Identify dependencies**: Think about what files and dependencies you have in the codebase that you want to include
3. **Use AI for brainstorming**: Turn on Ask/Chat mode and dump your context to get structured feedback

#### Example Planning Prompt

```
I need to add user authentication to my web app. Here's what I have:

Context:
- Next.js app with TypeScript
- Already using Prisma for database
- Want to implement OAuth with Google and GitHub
- Need protected routes and user sessions

Files to consider:
- `/lib/auth.ts` (doesn't exist yet)
- `/pages/api/auth/` folder structure
- `/components/LoginButton.tsx`
- `/middleware.ts` for route protection

Dependencies I know I'll need:
- NextAuth.js for OAuth handling
- @next-auth/prisma-adapter for database integration

Help me create a step-by-step implementation plan, breaking this down into logical phases that I can tackle incrementally.
```

### Planning Best Practices

- **Start with the end goal**: Clearly define what success looks like
- **Break into phases**: Divide complex features into logical, testable increments  
- **Identify integration points**: Note where new code will interact with existing systems
- **Consider edge cases early**: Think through error states and boundary conditions
- **Plan for testing**: Include validation steps for each phase
- **Document assumptions**: Note any assumptions about user behavior or system constraints

See our [planning templates](planning/) for structured approaches to feature planning and development workflows.

## Custom Instructions for AI Assistants

By adding custom instructions to your repository, you can guide Copilot on how to understand your project and how to build, test and validate its changes.

If Copilot is able to build, test and validate its changes in its own development environment, it is more likely to produce good pull requests which can be merged quickly.

Add instructions to a .github/copilot-instructions.md file in the repository. For more information, see Adding repository custom instructions for GitHub Copilot.

Here is an example of effective instructions: [copilot-instructions.md](custom-instructions/copilot-instructions.md)


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