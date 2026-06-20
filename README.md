# Expense-Keeper

Plataforma MVP para la gestión y control de finanzas personales.

## Equipo

| Integrante | Rol |
|---|---|
| Eréndira Becerra A. | Product Owner / Scrum Master |
| Alejandro Juárez M. | Dev Team |

---

## Prototipo Interactivo

> **Acceso público al prototipo:** https://ere8712.github.io/Expense-Keeper/prototypes/Expense-Keeper.html

---

## Visión del MVP

**Problema:** Muchas personas tienen dificultades para llevar un control adecuado de sus gastos personales, lo que provoca desorganización financiera, pagos olvidados y problemas para administrar su dinero correctamente.

**Propuesta de valor:** Expense-Keeper ofrece una plataforma sencilla e intuitiva que permite registrar, organizar y visualizar gastos personales, ingresos y métodos de pago en un solo lugar.

**Alcance crítico del MVP:**
1. Registro de ingresos y gastos.
2. Clasificación de gastos por categorías predefinidas.
3. Visualización del historial financiero cronológico.
4. Gestión básica de métodos de pago (Efectivo y Tarjetas).

---

## Estructura del Repositorio

```
Expense-Keeper/
├── README.md                          ← Portada del proyecto
├── docs/
│   ├── business/
│   │   └── historias_usuario.md       ← HU con Criterios Gherkin (Sesión 3)
│   ├── design/
│   │   ├── sitemap.png                ← Mapa jerárquico de pantallas (Sesión 4)
│   │   └── user_flows.pdf             ← Diagramas de flujo de navegación (Sesión 4)
│   └── architecture/
│       ├── README.md                  ← Métodos HTTP / Swagger (Sesión 5)
│       └── contratos/
│           ├── registro_gasto.json    ← Contrato de datos: registro de gasto (Sesión 5)
│           └── nuevo_metodo_pago.json ← Contrato de datos: método de pago (Sesión 5)
├── management/                        ← Documentos de gestión del proyecto
└── prototypes/
    └── Expense-Keeper.html            ← Prototipo interactivo principal
```

---

## Gestión del Proyecto

| Herramienta | Enlace |
|---|---|
| Tablero Kanban (Jira) | [Ver tablero](https://bujece-devs.atlassian.net/jira/software/projects/KAN/boards/1) |
| Repositorio GitHub | [Expense-Keeper](https://github.com/Ere8712/Expense-Keeper) |

---

## Historial de Sprints

### Sprint 1 — Base y Configuración
- Configuración del repositorio en GitHub.
- Documentación de la visión del MVP, alcance y roles.

### Sprint 2 — Planeación
- Configuración del tablero Kanban en Jira.
- Definición de Historias de Usuario y tareas técnicas.

### Sprint 3 — Prototipado y Diseño
- Desarrollo del prototipo interactivo en HTML5 + Tailwind CSS (estética Glassmorphism).
- Creación de artefactos de diseño: `sitemap.png` y `user_flows.pdf`.

### Sprint 4 — Arquitectura de Datos
- Modelado de contratos JSON para las pantallas clave.
- Documentación de endpoints y métodos HTTP bajo estándar Swagger.

### Sprint 5 — Cierre y Calidad _(Sprint actual)_
- Reorganización de la estructura del repositorio según estándar de entrega final.
- Conversión de Criterios de Aceptación a formato Gherkin.
- Publicación del prototipo interactivo con enlace público.
- Cierre formal del Sprint en Jira y trazabilidad cruzada.
