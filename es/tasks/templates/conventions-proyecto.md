# 📐 Convenciones de desarrollo del proyecto

Este documento define las convenciones internas de desarrollo para mantener consistencia, legibilidad y calidad técnica dentro del proyecto.

---

## 📁 Estructura de carpetas recomendada

```
src/
├── components/           # Componentes reutilizables
├── features/             # Módulos funcionales por dominio (auth, dashboard, etc.)
├── lib/                  # Funciones y utilidades compartidas
├── pages/                # Rutas (Next.js o frameworks similares)
├── styles/               # Archivos CSS/Tailwind
├── hooks/                # Custom hooks
└── types/                # Tipos globales (TypeScript)
```

---

## 📄 Nombres de archivos y componentes

| Elemento    | Convención                | Ejemplo             |
| ----------- | ------------------------- | ------------------- |
| Componentes | PascalCase                | `UserCard.tsx`      |
| Hooks       | camelCase, prefijo `use`  | `useAuth.ts`        |
| Archivos    | kebab-case                | `user-card.tsx`     |
| Test files  | mismo nombre + `.test.ts` | `user-card.test.ts` |

---

## 🌐 Idioma

- Todos los **nombres de archivos, variables, funciones y comentarios** deben estar en **inglés**.
- El contenido visible al usuario puede estar en múltiples idiomas (`i18n`).
- Documentación interna del equipo puede estar en español si se especifica.

---

## 🧪 Testing

- Preferencia por `unit tests` usando **Jest** o **Vitest**
- Cada hook, utilidad o componente debe tener su test cuando aplique
- Tests deben residir junto al archivo fuente o en `/__tests__/`

---

## 🧹 Estilo y lint

- Usar `eslint` con reglas adaptadas a TypeScript + React
- Usar `prettier` para formateo automático
- `lint-staged` + `husky` en pre-commits (opcional pero recomendado)

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

## 🔁 Pull Requests

- Título claro, breve y en presente
- Descripción con **qué, por qué y cómo**
- Enlazar la tarea si aplica (Jira, Linear, GitHub Issues...)
- Acompañar de tests o screenshots si es UI

---

## 🧠 Revisión de código

- Código claro > código listo
- Nombres descriptivos > abreviaturas
- Evita repetir lógica → crear utilidades/herramientas
- Si un cambio rompe un patrón existente, debe justificarse

---

## 📝 Documentación

- Documentar decisiones importantes en un archivo `docs/` o en `README.md`
- Siempre que agregues algo que impacte a otros desarrolladores, documenta

---

Made with ❤️ para facilitar el desarrollo limpio y colaborativo
