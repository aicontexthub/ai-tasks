# 🚀 Starting a New Project Using AI Tasks Examples

This guide explains how to use an existing AI Tasks example to bootstrap a real project with pre-defined context, structure, and reusable tasks.

---

## 1️⃣ Choose a base example

From the `/examples/` folder, pick the tech stack that matches your project:

| Stack            | Path                       |
| ---------------- | -------------------------- |
| React + Next.js  | `examples/react-frontend/` |
| Python + FastAPI | `examples/python-api/`     |

---

## 2️⃣ Copy the base task structure and templates

Before copying example tasks, copy the reusable templates and conventions from the English version:

```bash
mkdir -p ./my-project/tasks/templates

# Copy templates and helpers
cp -r en/tasks/templates/* ./my-project/tasks/templates/
cp en/tasks/review-template.md ./my-project/tasks/
cp en/tasks/task-help.md ./my-project/tasks/
```

---

## 3️⃣ Copy example task files

Now copy the task examples from the stack-specific folder:

```bash
mkdir -p ./my-project/tasks

# Copy example tasks
cp examples/react-frontend/task-*.yaml ./my-project/tasks/

# (Optional) Copy reviews
cp examples/react-frontend/review-*.md ./my-project/tasks/
```

---

## 4️⃣ Initialize your project context

Use the first context task from the example:

```bash
task configure-project: ./tasks/task-001-define-project-context.yaml
```

This will generate:

- `contexts/project.md`
- `contexts/stack.md`
- `contexts/mvp.md`
- Optionally: `contexts/ui-components/*` if the project uses a design system like shadcn/ui

These files give your agent a solid technical foundation to work with.

---

## 5️⃣ Start working with structured tasks

Now you're ready to begin building your project:

- Use `task new:` to create new detailed tasks
- Use `task-template-avanzado.yaml` to structure them
- Review output with `review-template.md`

---

## 🧠 Why use this workflow?

- ✅ Stop repeating project context in every prompt
- ✅ Prevent inconsistent or ad-hoc code from the AI
- ✅ Write reusable, versioned, and traceable instructions
- ✅ Collaborate with AI (and humans) like a real team

> Think of it as version-controlled prompt engineering — made for developers.

---

Made with ❤️ by [AI Context Hub](https://github.com/aicontexthub)

---

## 💬 Want to collaborate?

This repo is part of the [aicontexthub](https://github.com/aicontexthub) GitHub organization.  
Feel free to open an issue, suggest improvements, or submit templates!
