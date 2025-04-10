# 📐 Convenciones – AI Tasks CLI

Este archivo define las convenciones internas para nombrar, estructurar y organizar las tareas (`tasks`) y sus archivos asociados dentro del repositorio `ai-tasks`.

---

## 🗂️ Estructura general

```
tasks/
├── templates/          # Plantillas reutilizables (.yaml, .txt, .md)
├── examples/           # Tareas ejecutadas en proyectos reales
├── reviews/            # Revisiones detalladas de tareas realizadas
├── CONVENTIONS.md      # Este archivo
├── task.config.json    # Configuración global
└── README.md           # Instrucciones principales del repositorio
```

---

## 📄 Convenciones de nombre de archivo

| Tipo de archivo        | Formato recomendado                  | Ejemplo                     |
| ---------------------- | ------------------------------------ | --------------------------- |
| Tarea (`task`)         | `task-<id>.yaml`                     | `task-001.yaml`             |
| Revisión (`review`)    | `review-task-<id>.md`                | `review-task-001.md`        |
| Plantilla (`template`) | `<nombre>.yaml` / `.txt` / `.md`     | `create-project.txt`        |
| Alias de tarea         | `task new:` / `task create-project:` | CLI-friendly, sin extensión |

---

## 📦 Extensiones de templates

| Extensión | Uso recomendado                                          |
| --------- | -------------------------------------------------------- |
| `.yaml`   | Plantillas 100% compatibles con YAML                     |
| `.txt`    | Plantillas dinámicas con condicionales (`{{#if}}`, etc.) |
| `.md`     | Documentación o plantillas de revisión (Markdown)        |

---

## 🌐 Política de idiomas

Este repositorio está escrito principalmente en español, pero optimizado para agentes de IA que operan mejor en inglés.

### 🧠 Variables de idioma en tareas

Cada `task.yaml` puede incluir:

```yaml
language: es # Idioma del input humano
output_language: es # Idioma esperado en la salida del agente
```

Esto permite a la IA:

- Traducir internamente al inglés para entender mejor la tarea
- Generar la salida final en español o inglés, según el valor de `output_language`

### ⚙️ Código siempre en inglés

- El código generado, nombres de archivo, estructuras y convenciones técnicas deben estar **siempre en inglés** para mantener compatibilidad y buenas prácticas.

---

## ⚙️ Configuración global – task.config.json

Puedes definir configuraciones predeterminadas para todo el sistema de tareas en el archivo `task.config.json`, ubicado en la raíz del repositorio.

Ejemplo:

```json
{
  "default_language": "es",
  "default_output_language": "es",
  "force_output_code_language": "en",
  "task_id_format": "task-###.yaml",
  "review_id_format": "review-task-###.md",
  "templates_path": "./templates",
  "examples_path": "./examples",
  "reviews_path": "./reviews",
  "project_context": "AI Context Hub"
}
```

Esto permite que los agentes IA, colaboradores o herramientas CLI respeten una configuración común y consistente.

---

## 💾 Recomendación: commits al finalizar tareas

Al finalizar cualquier tarea o microtarea generada por IA o colaborador, se recomienda incluir al final del mensaje:

```
Don't forget to commit!
```

Y sugerir un comando útil como referencia:

```bash
git add tasks/examples/ai-context-hub/task-003-implement-dashboard-protection.yaml
git commit -m "feat: implement dashboard route protection"
```

### ✅ Convención sugerida para prefijos de commits

| Prefijo     | Uso                                   |
| ----------- | ------------------------------------- |
| `feat:`     | Nueva funcionalidad                   |
| `fix:`      | Corrección de errores                 |
| `docs:`     | Cambios en documentación              |
| `chore:`    | Tareas de mantenimiento/config        |
| `refactor:` | Refactor interno sin cambio de lógica |
| `test:`     | Cambios o adición de tests            |

> Aunque no es obligatorio, seguir esta convención mejora la trazabilidad y legibilidad del historial de cambios.

---

## 🧠 Recomendaciones adicionales

- Los `id` deben ser numéricos y secuenciales (`001`, `002`, `003`) para orden natural.
- Los `review` deben ir siempre en `reviews/`.
- Los `examples` se agrupan por proyecto dentro de `examples/`.
- Toda tarea técnica significativa debe tener su revisión (`review-task-xxx.md`).
- Los archivos `.md` y `.yaml` deben ser claros, sin lógica oculta, y 100% copiable.

---

## 📌 Notas finales

Este sistema está optimizado para el flujo de trabajo de [AI Context Hub](https://www.aicontexthub.com), pero puede adaptarse fácilmente a cualquier entorno de desarrollo asistido por IA.
