## Step 4: Start working with Claude Code

Every project that uses Claude Code should include a `CLAUDE.md` file.

### What is `CLAUDE.md`?
`CLAUDE.md` is a configuration and instruction file that helps guide Claude’s behavior when working on your project.

It can include:
- Project context
- Coding guidelines
- Instructions and preferences
- Repeated workflows or patterns

---

### Working with an existing project

If you're working with an existing codebase, run:
```
/init
```

This will automatically generate a `CLAUDE.md` file.

**Important:**
Review and refine this file carefully to ensure it accurately reflects your project and expectations.

---

### Starting a new project

If you're starting from scratch, create the `CLAUDE.md` file yourself and define:
- What the project does
- How you want Claude to behave
- Any constraints or best practices

---

### 💡 Pro Tip

If you find yourself repeating the same instructions multiple times, add them to `CLAUDE.md`.

This ensures Claude consistently follows your preferences and improves output quality over time.

---

## Step 5: Write effective prompts

To get the best results from Claude Code, it's important to write clear and focused prompts.

### Best practices for prompting

- **Be specific**: Clearly describe what you want (e.g., "Refactor this function for readability")
- **Provide context**: Explain what the code is part of or what you're trying to achieve
- **Define constraints**: Mention frameworks, languages, or patterns if relevant
- **Iterate**: Improve your prompt based on the response you get

---

### 🎯 Focus the conversation on specific files

When working with a codebase, explicitly reference the file you want Claude to focus on.

**Examples:**
- "In `auth_service.py`, improve the error handling logic"
- "Refactor the function in `user_controller.ts` to make it more modular"
- "Add validation to the form in `signup.jsx`"

This helps Claude understand exactly where to look and produces more accurate results.

---

### 💡 Pro Tip

If you're repeatedly giving similar instructions (e.g., coding style, naming conventions),
add them to `CLAUDE.md` instead of rewriting them every time.
