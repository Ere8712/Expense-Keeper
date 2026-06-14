# Expense-Keeper
Proyecto de gestión y control de gastos personales.

## Integrantes
- ERENDIRA BECERRA A.
- ALEJANDRO JUAREZ M.

## Roles

### ERENDIRA BECERRA
- Product Owner (PO)
- Scrum Master

### ALEJANDRO JUAREZ
- Dev Team

---

# Visión del MVP

## Problema (Pain Point)
Muchas personas tienen dificultades para llevar un control adecuado de sus gastos personales, lo que provoca desorganización financiera, pagos olvidados y problemas para administrar su dinero correctamente.

## Propuesta de Valor
Expense-Keeper ofrecerá una plataforma sencilla e intuitiva que permitirá registrar, organizar y visualizar gastos personales, ingresos y métodos de pago en un solo lugar.

## Alcance Crítico (MVP)
1. Registro de ingresos y gastos.
2. Clasificación de gastos por categorías.
3. Visualización del historial financiero.
4. Gestión básica de métodos de pago.

## Métrica de Éxito
El MVP será exitoso si los usuarios logran tener un mejor control y organización de sus gastos personales mediante el uso constante de la plataforma.

---

# Estructura del Proyecto

- `/management` → Documentos de gestión y planeación.
- `/docs` → Documentación técnica y de ingeniería.
  - `/docs/design` → Contiene los entregables de diseño, incluyendo el mapa de navegación (`sitemap.png`) y los diagramas lógicos (`user_flows.pdf`).
  - `/docs/architecture` → Contiene el modelado de datos en formato JSON y la documentación de métodos HTTP/API.
- `/prototypes` → Prototipos, diagramas y recursos visuales. Contiene el archivo interactivo en código nativo `Expense-Keeper.html`.

---

## Historial de Avance y Sprints

### Sprint 1 — Base y Configuración
- Configuración inicial del repositorio en GitHub.
- Documentación de la visión del MVP, alcance crítico y definición de roles.

### Sprint 2 — Planeación y Diseño Lógico
- Configuración del tablero Kanban y definición detallada de las tareas e historias de usuario en Jira.
- Creación de los artefactos de diseño: mapa de navegación (`sitemap.png`) y flujos lógicos (`user_flows.pdf`).

### Sprint 3 — Prototipado
- Desarrollo de la interfaz de usuario para el MVP.
- Creación del prototipo interactivo web directamente en código utilizando HTML5 y Tailwind CSS.
- Maquetación de las vistas de Login, Resumen de Saldo, Historial Cronológico, Gestión de Tarjetas y el Modal de Registro.

### Sprint 4 — Sprint Actual (Arquitectura de Datos)
- **Objetivo principal:** Modelar la estructura de datos y definir la comunicación entre la interfaz y el servidor.
- Escaneo de campos de captura desde el prototipo HTML y modelado de datos de transmisión en formato JSON (`registro_gasto.json` y `nuevo_metodo_pago.json`).
- Definición y documentación de los métodos HTTP (GET, POST) y endpoints bajo estándares REST para las funcionalidades críticas del MVP.

---

## Gestión del Proyecto

| Herramienta | Enlace |
|---|---|
| Tablero Kanban (Jira) | [Ver tablero](https://bujece-devs.atlassian.net/jira/software/projects/KAN/boards/1?jql=&atlOrigin=eyJpIjoiMGYzOTU1NzEwZWNiNDU4MTliYTVjZGVmNWQzNTU3MGMiLCJwIjoiaiJ9) |
| Repositorio GitHub | [Expense-Keeper](https://github.com/Ere8712/Expense-Keeper) |

### Sprint actual
Sprint 4 — Sesión de Arquitectura Activa
