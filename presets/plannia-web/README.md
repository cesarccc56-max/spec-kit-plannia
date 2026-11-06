# Plannia Web preset

Proceso Plannia para sitios web de clientes sobre Spec Kit.

## Que agrega

| Plantilla | Estrategia | Contenido |
| --- | --- | --- |
| `constitution-template` | replace | Constitucion web: negocio primero, WCAG 2.2 AA, Core Web Vitals, OWASP, stack minimo, sin estetica generica de AI, 9 fases y Definition of Done |
| `spec-template` | append | Objetivo, KPI, accion principal, audiencia, sitemap, alcance, restricciones y referencias |
| `plan-template` | append | Stack justificado, DESIGN.md, plan de eventos, JSON-LD, presupuestos de calidad y seguridad |
| `tasks-template` | append | Criterio de salida por tarea, fase QA y fase de lanzamiento |

No reemplaza comandos: el flujo `/speckit.*` es el oficial, solo cambian las plantillas que esos comandos llenan.

## Uso

```bash
specify init mi-sitio --integration claude --preset plannia-web
# o en un proyecto existente
specify preset add plannia-web
```
