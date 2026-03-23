## Step 5: Write effective prompts

To get the best results from Claude Code, it's important to write clear, structured, and contextual prompts.

### Best practices for prompting

- **Be clear and explicit**  
  Clearly state what you want Claude to do. Avoid vague instructions.  
  - ❌ "Improve this"  
  - ✅ "Refactor this function to improve readability and reduce duplication"

- **Provide context upfront**  
  Explain what the code does and what you're trying to achieve.  
  Claude performs significantly better when it understands the bigger picture.  
  - Example: "This service handles user authentication. Optimize it for better error handling and logging."

- **Break down complex tasks**  
  For larger requests, guide Claude step-by-step instead of asking for everything at once.  
  - Example:  
    1. Analyze the current implementation  
    2. Suggest improvements  
    3. Refactor the code  

- **Specify constraints and preferences**  
  Mention technologies, patterns, or limitations.  
  - Example: "Use FastAPI best practices" / "Avoid external dependencies"

- **Ask for reasoning when needed**  
  If you want to understand decisions:  
  - "Explain why you chose this approach"

- **Iterate and refine**  
  Treat prompting as an iterative process. Improve your instructions based on the output you get.

---

### 🎯 Focus Claude on specific files

When working with a codebase, explicitly reference the file you want Claude to focus on using `@`.

**Examples:**
- "@auth_service.py improve the error handling logic"
- "@user_controller.ts refactor this to be more modular"
- "@signup.jsx add validation to the form"

Using `@filename` helps Claude narrow down the context and provide more accurate, relevant results.

---

### 💡 Pro Tip

If you repeatedly give the same instructions (e.g., coding style, naming conventions, architecture decisions),
add them to `CLAUDE.md` instead of repeating them in every prompt.

This allows Claude to apply your preferences consistently across all interactions.

---

## Step 6: Build trust and learn the tool

To work effectively with Claude Code, it's important to build trust in the tool and understand how it behaves.

### Start with something you already know

Pick a component, service, or piece of code that you are already familiar with, and ask Claude to explain it.

**Examples:**
- "@auth_service.py explain how this service works"
- "@payment_handler.ts describe the system design and flow"
- "@user_model.py what is the logic behind this implementation?"

---

### What to look for

When reviewing Claude’s response, evaluate:
- Does it correctly understand the system?
- Does it explain the flow clearly?
- Does it miss anything important?
- Does it make incorrect assumptions?

---

### 💡 Why this matters

By starting with familiar code, you can:
- Calibrate Claude’s level of understanding  
- Learn how to phrase better prompts  
- Identify strengths and limitations  
- Build confidence in using the tool on real tasks  

---

### 💡 Pro Tip

If Claude is partially correct, guide it:
- "You're close, but you're missing X"
- "Take into account that this service also handles Y"

Treat it as a collaborative iteration process — the more you guide it, the better it performs.
