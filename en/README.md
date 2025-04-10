# 🧠 AI Tasks

Repository of templates and technical tasks for organizing and executing AI-assisted workflows (ChatGPT, Cursor, Claude, etc).  
This system allows structuring technical contexts, detailed tasks, and reviews for use in any project.

---

## 🎯 Objective

Centralize a set of reusable `tasks` for:

- Creating base technical contexts for projects
- Generating detailed tasks for AI agents
- Reviewing and documenting completed tasks
- Maintaining clear naming and structure conventions

This system is used by [AI Context Hub](https://www.aicontexthub.com), but can be applied to any AI-assisted development environment.

---

## 🧩 What does this repository contain?

```
ai-tasks/
├── CONVENTIONS.md                      # 📐 Structure, language, commit conventions and more
├── README.md                           # 🧠 Clear instructions for using the task system
├── task.config.json                    # ⚙️ Global system configuration (languages, paths, etc.)

├── templates/                          # 🧩 Reusable templates
│   ├── create-project.txt              # Base project context generator
│   ├── improve-with-ai.yaml            # Technical improvement tasks with AI assistance
│   ├── review-template.md              # Base for reviewing completed tasks
│   ├── setup-ui-context.yaml           # UI system documentation (shadcn/ui, variants)
│   ├── task-help.md                    # Table of available commands
│   ├── task-review.md                  # Structured review Markdown template
│   └── task-template-avanzado.yaml     # Complete template for complex technical tasks

├── examples/                           # 🧪 Real tasks executed by project
│   └── ai-context-hub/
│       ├── task-001-generate-readme.yaml
│       └── task-003-implement-dashboard-protection.yaml ✅ updated

├── reviews/                            # ✅ Technical reviews of completed tasks
│   ├── review-task-001.md
│   └── review-task-002.md

```

---

## 🚀 How to use it?

This repository doesn't require installation. You just need to:

1. Copy the `tasks/` folder to your project (or reference this repo).
2. Execute tasks manually or from your AI tool.
3. Follow the conventions in the `CONVENTIONS.md` file.

### 📄 Usage examples

- **Create a new project context**  
  Use the `templates/create-project.txt` file to launch interactive questions and generate `project.md`, `stack.md`, `mvp.md`.

- **Generate a new technical task**  
  Execute a `task new:` in your AI system, and save as `task-xxx.yaml`.

- **Review an executed task**  
  Use `templates/review-template.md` to record observations as `review-task-xxx.md`.

- **View available commands**  
  Check `templates/task-help.md` or create your own list in the project.

---

## 📐 Conventions

Check [`CONVENTIONS.md`](./CONVENTIONS.md) for:

- File naming (`task-001.yaml`, `review-task-001.md`)
- Folder structure
- How to organize your tasks and templates

---

## 📎 Recommended for

- Agents like ChatGPT, Cursor, Claude, Perplexity
- Workflows requiring clear and persistent technical context
- Teams wanting to maintain standards in AI-generated tasks

---

Made with ❤️ to improve human + AI collaboration
