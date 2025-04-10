# 🧠 AI Tasks

Repositorio de plantillas y tareas técnicas para organizar y ejecutar flujos de trabajo asistidos por IA (ChatGPT, Cursor, Claude, etc).  
Este sistema permite estructurar contextos técnicos, tareas detalladas y revisiones para usarlas en cualquier proyecto.

---

## 🎯 Objetivo

Centralizar un conjunto de `tasks` reutilizables para:

- Crear contextos técnicos base de proyectos
- Generar tareas detalladas para agentes IA
- Revisar y documentar tareas completadas
- Mantener convenciones claras de nombre y estructura

Este sistema es utilizado por [AI Context Hub](https://www.aicontexthub.com), pero puede aplicarse a cualquier entorno de desarrollo asistido por IA.

---

## 🧩 ¿Qué contiene este repositorio?

```
ai-tasks/
├── CONVENTIONS.md                      # 📐 Convenciones de estructura, idioma, commits y más
├── README.md                           # 🧠 Instrucciones claras de uso del sistema de tareas
├── task.config.json                    # ⚙️ Configuración global del sistema (idiomas, paths, etc.)

├── templates/                          # 🧩 Plantillas reutilizables
│   ├── create-project.txt              # Generador de contexto base de proyectos
│   ├── improve-with-ai.yaml            # Tareas de mejora técnica con ayuda de IA
│   ├── review-template.md              # Base para revisar tareas completadas
│   ├── setup-ui-context.yaml           # Documentación del sistema UI (shadcn/ui, variantes)
│   ├── task-help.md                    # Tabla con comandos disponibles
│   ├── task-review.md                  # Plantilla estructurada de revisión Markdown
│   └── task-template-avanzado.yaml     # Plantilla completa para tareas técnicas complejas

├── examples/                           # 🧪 Tareas reales ejecutadas por proyecto
│   └── ai-context-hub/
│       ├── task-001-generate-readme.yaml
│       └── task-003-implement-dashboard-protection.yaml ✅ actualizado

├── reviews/                            # ✅ Revisiones técnicas de tareas completadas
│   ├── review-task-001.md
│   └── review-task-002.md

```

---

## 🚀 ¿Cómo se usa?

Este repositorio no necesita instalación. Solo debes:

1. Copiar la carpeta `tasks/` a tu proyecto (o referenciar este repo).
2. Ejecutar tareas manualmente o desde tu herramienta de IA.
3. Seguir las convenciones del archivo `CONVENTIONS.md`.

### 📄 Ejemplos de uso

- **Crear un nuevo contexto de proyecto**  
  Usa el archivo `templates/create-project.txt` para lanzar preguntas interactivas y generar `project.md`, `stack.md`, `mvp.md`.

- **Generar una nueva tarea técnica**  
  Ejecuta un `task new:` en tu sistema con IA, y guarda como `task-xxx.yaml`.

- **Revisar una tarea ejecutada**  
  Usa `templates/review-template.md` para registrar observaciones como `review-task-xxx.md`.

- **Ver comandos disponibles**  
  Consulta `templates/task-help.md` o crea tu propia lista en el proyecto.

---

## 📐 Convenciones

Consulta [`CONVENTIONS.md`](./CONVENTIONS.md) para:

- Nombres de archivo (`task-001.yaml`, `review-task-001.md`)
- Estructura de carpetas
- Cómo organizar tus tareas y plantillas

---

## 📎 Recomendado para

- Agentes como ChatGPT, Cursor, Claude, Perplexity
- Flujos de trabajo que requieran contexto técnico claro y persistente
- Equipos que deseen mantener estándares en tareas generadas con IA

---

Made with ❤️ para mejorar la colaboración humano + IA
