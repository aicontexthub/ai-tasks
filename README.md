# 🧠 AI Tasks

> A lightweight, multilingual system for creating, organizing, and reviewing AI-assisted development tasks — built for developers who want clarity, consistency, and control when working with AI.

---

## ❓ Why this project exists

Working with AI (ChatGPT, Cursor, Claude, Copilot...) can be powerful — but also frustrating.  
You often face the same issues:

- Repeating your project context in every prompt
- Getting inconsistent or duplicated code
- Receiving vague, incomplete, or unstructured results
- Struggling to define clear instructions for agents

**AI Tasks** solves this by introducing a reusable, versioned system of structured tasks and context.  
It's like version control, but for your prompts, logic, and standards — built for reuse, precision, and collaboration.

---

## 🧩 What is this repository?

This is the canonical repository for the **AI Tasks format** used in [AI Context Hub](https://www.aicontexthub.com). It provides:

- 📁 Examples of well-defined tasks in YAML format
- 🧩 Templates to create tasks, project context, and reviews
- 🌐 Multilingual folders (`es/`, `en/`, etc.) with localized documentation

This repo is not a CLI (yet), but can be used manually, via agents, or integrated into your own tooling.

---

## 🔧 How does it work?

1. Copy the `/tasks/` folder into your project.
2. Use `create-project.txt` to generate context interactively.
3. Write new structured tasks using `task-template-avanzado.yaml`.
4. Review executed tasks with `review-template.md`.
5. Add your own structure, steps, criteria, and context for agents.

---

## 🌍 Languages

This repository supports multiple languages:

- 🇪🇸 [Español](./es/README.md)
- 🇬🇧 [English](./en/README.md)

More coming soon: Portuguese, French, Italian...

---

## 🔮 What's next?

These are ideas we would love to see evolve within this system — feel free to contribute:

- 🧠 AI-powered task review system
- 🛠️ CLI interface to launch tasks and auto-generate files
- 🔄 Integration with local agents (ChatGPT, Cursor, Claude)
- 🧱 Templates for stack-specific projects (React, Python, Laravel, etc.)
- 🗂️ Import/export via `.task.yaml` format across editors or tools

You’re welcome to open an issue or submit a pull request if you’d like to help build any of these!

---

## 🧪 Examples by stack

Real project examples are located in the root `/examples` folder, grouped by technology.

| Stack           | Path                        | Description                    |
| --------------- | --------------------------- | ------------------------------ |
| React + Next.js | `/examples/react-frontend/` | Modern frontend SaaS project   |
| Python backend  | `/examples/python-api/`     | FastAPI-based task definitions |
| CLI utilities   | `/examples/dev-cli/`        | Tasks for Node/Python tool dev |

> All examples use **English** for compatibility with AI agents.

Want to add a new one? Fork this repo, create a folder inside `/examples/`, and follow the naming convention: `task-###.yaml`.

---

## 💬 Want to collaborate?

This repo is part of the [aicontexthub](https://github.com/aicontexthub) GitHub organization.  
Feel free to open an issue, suggest improvements, or submit templates!

---

Made with ❤️ to help humans and AI build better software together.

---

### ☕️ Support This Project

If you find **AI Tasks** useful and want to support continued development:

<a href="https://www.buymeacoffee.com/aicontexthub" target="_blank">
  <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=☕&slug=aicontexthub&button_colour=FFDD00&font_colour=000000&font_family=Arial&outline_colour=000000&coffee_colour=ffffff" alt="Buy Me A Coffee" />
</a>

> It helps keep the ideas flowing and the context structured ☺️
