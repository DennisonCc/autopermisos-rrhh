# PROCESO DEL EQUIPO

# PARTE A. METODOLOGÍA Y FLUJO

## Metodología

El equipo utilizará Scrum con iteraciones de dos semanas debido a que el proyecto necesita validaciones frecuentes y entregas incrementales.

## Flujo del Sprint

| Actividad | Entrada | Salida | Responsable |
|------------|------------|------------|------------|
| Planificar Sprint | Product Backlog | Sprint Backlog | Líder |
| Desarrollo | Historia asignada | Rama y commits | Desarrollador |
| Revisión | Pull Request | Correcciones o aprobación | Calidad |
| Integración | PR aprobado | Merge a main | DevOps |
| Revisión Sprint | Incremento funcional | Retroalimentación | Equipo |
| Retrospectiva | Métricas sprint | Acciones mejora | Líder |

## Eventos

| Evento | Cuándo | Duración | Participantes | Evidencia |
|----------|----------|----------|----------|----------|
| Sprint Planning | Inicio Sprint | 30 min | Equipo | Project |
| Seguimiento | Semanal | 15 min | Equipo | Issues |
| Sprint Review | Fin Sprint | 20 min | Equipo | Pull Requests |
| Retrospectiva | Fin Sprint | 20 min | Equipo | Acta |

# PARTE B. ROLES Y RESPONSABILIDADES

## Roles

| Rol | Integrante | Responsabilidades |
|------|------|------|
| Líder | Dennison Chalacan | Planificar y coordinar |
| Analista | Jeffrey Manobanda | Gestionar requisitos |
| Calidad y DevOps | Fernando Tipan | Revisar calidad y despliegues |
| Product Owner | Docente | Validar entregables |

## Matriz RACI

| Actividad | Docente | Líder | Analista | Calidad |
|------------|------------|------------|------------|------------|
| Priorizar backlog | A | R | C | I |
| Crear historias | C | I | R | C |
| Programar funcionalidades | I | C | R | R |
| Revisar PR | I | C | C | R |
| Fusionar PR | I | I | C | R |
| Gestionar tablero | I | R | C | C |
| Realizar retrospectiva | I | R | C | C |
| Aceptar incremento | A | C | I | I |

## Rotación

| Sprint | Líder | Analista | Calidad |
|----------|----------|----------|----------|
| 1 | Dennison | Jeffrey | Fernando |
| 2 | Jeffrey | Fernando | Dennison |
| 3 | Fernando | Dennison | Jeffrey |
| 4 | Dennison | Jeffrey | Fernando |
| 5 | Jeffrey | Fernando | Dennison |
| 6 | Fernando | Dennison | Jeffrey |
| 7 | Dennison | Jeffrey | Fernando |
| 8 | Jeffrey | Fernando | Dennison |

# PARTE C. ARTEFACTOS

## Catálogo de Artefactos

| Artefacto | Propósito | Ubicación |
|------------|------------|------------|
| Product Backlog | Historias priorizadas | GitHub Issues |
| Sprint Backlog | Gestión Sprint | GitHub Project |
| Requisitos | RF y RNF | docs/02-requisitos |
| Casos de Uso | Especificaciones funcionales | docs/03-modelado |
| PROCESO.md | Metodología | docs/proceso |
| Riesgos | Gestión de riesgos | docs/01-inicio |
| Retrospectivas | Mejora continua | docs/proceso/retros |
| Incremento | Software funcional | main |

## Definición de Terminado

1. Código compilado.
2. Criterios de aceptación cumplidos.
3. Pull Request revisado.
4. Documentación actualizada.
5. Sin errores críticos.
6. PR aprobado.
7. Issue cerrado.

# PARTE E. FLUJO DE RAMAS

## Comparación

| Criterio | Git Flow | GitHub Flow | Trunk Based |
|------------|------------|------------|------------|
| Complejidad | Alta | Baja | Media |
| Equipo pequeño | Regular | Excelente | Buena |
| Frecuencia entrega | Media | Alta | Muy Alta |
| Conflictos | Medio | Bajo | Medio |

## Estrategia Seleccionada

GitHub Flow fue seleccionado debido al tamaño del equipo y la necesidad de realizar integraciones frecuentes.

## Convenciones

| Elemento | Convención |
|------------|------------|
| Rama | feature/número-descripción |
| Commit | feat:, fix:, docs: |
| PR | tipo: descripción |
| Merge | Squash and Merge |
| Versión | SemVer |

## Flujo

Issue → Rama → Commit → Pull Request → Revisión → Merge → Release