# 🎓 Proyecto Intermodular 2DAM — Propuesta de Ideas

> Repositorio de trabajo para la elección, planificación y desarrollo del Proyecto Intermodular de 2DAM.

---

## 👥 Equipo

| Nombre   | Rol propuesto     | GitHub |
|----------|-------------------|--------|
| Samuel   | Programador/Lider | [Enlace](https://github.com/TheYinYan) |
| Mari Paz | Programador       | [Enlace](https://github.com/mpjmar)    |

> Los roles son orientativos y se pueden rotar durante el proyecto.

---

## 🎯 Objetivo del Proyecto Intermodular

Diseñar y desarrollar una aplicación completa que integre los conocimientos de las asignaturas del ciclo:

- **Acceso a Datos** → base de datos real, relaciones, consultas.
- **Desarrollo de Interfaces** → frontend funcional y usable.
- **Programación de Servicios y Procesos** → API REST, tareas programadas, consumo de servicios externos.
- **Sistemas de Gestión Empresarial** → lógica de negocio, roles, flujos.
- **Programación** → backend en Java con buenas prácticas.

**Requisitos mínimos que debe cumplir la idea elegida:**
- Backend en **Java** con API REST.
- Base de datos **relacional** (MySQL / PostgreSQL).
- Frontend que consuma la API (Angular, JS/TS, etc.).
- Autenticación de usuarios.
- Al menos **una** de estas: consumo de API externa, tareas programadas, roles/permisos, subida de archivos.

---

## 💡 Ideas Propuestas

A continuación, 5 ideas **totalmente nuevas** (no son ampliaciones de proyectos previos del equipo). Se describen con el mismo formato para poder compararlas.

---

### 🎮 Idea 1 — "Rincón Gamer": Biblioteca personal de videojuegos

**Descripción:**
App web donde cada usuario registra los videojuegos que tiene, en qué plataforma, si los ha terminado, su puntuación y una reseña corta. Se puede filtrar por plataforma, género o estado (jugando / terminado / pendiente).

**Funcionalidades clave:**
- Registro y login de usuarios.
- CRUD de videojuegos personales.
- Filtros por plataforma, género y estado.
- Reseña y puntuación por juego.
- Autocompletado de datos del juego usando la API pública de **RAWG**.

**Tecnologías previstas:**
- Backend: Java + Spring Boot.
- Base de datos: MySQL/PostgreSQL (usuarios, juegos, plataformas, reseñas).
- Frontend: Angular o JS/TS.
- API externa: RAWG.

**Asignaturas que cubre:**
- Acceso a Datos (relaciones N:M, consultas).
- Desarrollo de Interfaces (listados, filtros, formularios).
- Programación de Servicios (API REST + consumo de API externa).
- Programación (backend Java).

**Puntos fuertes:**
- Tema atractivo y cercano.
- API externa que da valor añadido.
- Fácil de escalar (logros, listas públicas, etc.).

**Riesgos:**
- Dependencia de una API externa (hay que manejar errores y límites).

---

### 🛒 Idea 2 — "Mi Mercadillo": Trueque entre estudiantes

**Descripción:**
Plataforma donde los usuarios publican objetos que ya no usan (libros, apuntes, componentes, periféricos) y otros pueden solicitar un intercambio. El dueño acepta o rechaza la solicitud.

**Funcionalidades clave:**
- Registro y login.
- Publicación de objetos con imagen, descripción y estado.
- Sistema de solicitudes con estados: pendiente / aceptada / rechazada.
- Historial de intercambios.
- Tarea programada que caduca solicitudes antiguas.

**Tecnologías previstas:**
- Backend: Java + Spring Boot.
- Base de datos: MySQL/PostgreSQL (usuario ↔ objeto ↔ solicitud).
- Frontend: Angular o JS/TS.
- Subida de imágenes (multipart).

**Asignaturas que cubre:**
- Acceso a Datos (transacciones, estados).
- Desarrollo de Interfaces (listados, detalle, formularios con imagen).
- Programación de Servicios (tareas programadas con hilos).
- Sistemas de Gestión Empresarial (flujo de negocio con reglas).
- Programación (backend Java).

**Puntos fuertes:**
- Lógica de negocio real (no es un CRUD plano).
- Muy presentable en la defensa.
- Tarea programada → toca Programación de Servicios.

**Riesgos:**
- Más complejo de modelar (estados, permisos).

---

### 📚 Idea 3 — "Mis Apuntes DAM": Gestor de apuntes y recursos

**Descripción:**
Espacio personal donde se guardan apuntes, enlaces, snippets de código y ejercicios, organizados por asignatura y etiquetas. Búsqueda por texto, filtros y favoritos.

**Funcionalidades clave:**
- Registro y login.
- CRUD de apuntes con etiquetas y asignatura.
- Búsqueda full-text.
- Editor de código con resaltado de sintaxis.
- Enlace público temporal para compartir un apunte.

**Tecnologías previstas:**
- Backend: Java + Spring Boot.
- Base de datos: MySQL/PostgreSQL (búsqueda con índices).
- Frontend: Angular o JS/TS + CodeMirror/Monaco.
- Tokens para enlaces públicos.

**Asignaturas que cubre:**
- Acceso a Datos (búsqueda, índices).
- Desarrollo de Interfaces (editor, filtros, búsqueda).
- Programación de Servicios (API REST, tokens).
- Programación (backend Java).

**Puntos fuertes:**
- Utilidad real para el propio equipo.
- Editor de código → muy vistoso.
- Se puede dockerizar y desplegar fácilmente.

**Riesgos:**
- El editor de código añade complejidad al frontend.

---

### 📋 Idea 4 — "Turnos y Tareas": Planificador de trabajos en grupo

**Descripción:**
App para organizar trabajos en grupo de clase: se crea un proyecto, se reparten tareas, se asignan responsables y fechas, y cada uno marca su progreso. El líder ve el estado global.

**Funcionalidades clave:**
- Registro y login con roles (líder / miembro).
- Tablero kanban (pendiente / en curso / hecho) con drag & drop.
- Asignación de tareas y fechas.
- Historial de cambios (auditoría).
- Notificaciones o recordatorios programados.

**Tecnologías previstas:**
- Backend: Java + Spring Boot + Spring Security.
- Base de datos: MySQL/PostgreSQL (roles, auditoría).
- Frontend: Angular + Angular CDK (drag & drop).
- Envío de emails o recordatorios programados.

**Asignaturas que cubre:**
- Acceso a Datos (relaciones, auditoría).
- Desarrollo de Interfaces (kanban, drag & drop).
- Programación de Servicios (tareas programadas, notificaciones).
- Sistemas de Gestión Empresarial (roles y permisos).
- Programación (backend Java).

**Puntos fuertes:**
- Proyecto colaborativo → encaja con "trabajo en equipo".
- Roles y permisos → toca seguridad.
- Visualmente muy atractivo (kanban).

**Riesgos:**
- Drag & drop y permisos requieren tiempo.

---

### 👕 Idea 5 — "¿Qué me pongo?": Armario virtual con recomendaciones

**Descripción:**
Se suben fotos de la ropa, se etiqueta (tipo, color, temporada) y la app sugiere combinaciones según el clima del día (API meteorológica) y la ocasión (formal, casual, deporte).

**Funcionalidades clave:**
- Registro y login.
- Subida de fotos de ropa con etiquetas.
- Filtros por tipo, color y temporada.
- Consumo de API meteorológica.
- Algoritmo simple de recomendación (reglas).

**Tecnologías previstas:**
- Backend: Java + Spring Boot + HttpClient.
- Base de datos: MySQL/PostgreSQL (imágenes o rutas).
- Frontend: Angular o JS/TS.
- API externa: OpenWeather u similar.

**Asignaturas que cubre:**
- Acceso a Datos (relaciones, imágenes).
- Desarrollo de Interfaces (tarjetas, filtros visuales).
- Programación de Servicios (consumo de API externa).
- Programación (backend Java).

**Puntos fuertes:**
- Idea original y cotidiana.
- El "algoritmo de recomendación" suena muy bien en la defensa.
- API externa → cubre servicios.

**Riesgos:**
- Subida y gestión de imágenes añade complejidad.

---

## 📊 Comparativa rápida

| Criterio | Idea 1 | Idea 2 | Idea 3 | Idea 4 | Idea 5 |
|----------|:------:|:------:|:------:|:------:|:------:|
| Facilidad de modelado | ✅ | ⚠️ | ✅ | ⚠️ | ⚠️ |
| API externa | ✅ | ❌ | ❌ | ❌ | ✅ |
| Roles/permisos | ❌ | ⚠️ | ❌ | ✅ | ❌ |
| Tareas programadas | ❌ | ✅ | ❌ | ✅ | ❌ |
| Subida de archivos | ❌ | ✅ | ⚠️ | ❌ | ✅ |
| Vistosidad en defensa | ✅ | ✅ | ✅ | ✅✅ | ✅✅ |
| Utilidad real para el equipo | ⚠️ | ✅ | ✅✅ | ✅✅ | ⚠️ |

> ✅ = punto fuerte · ⚠️ = punto medio · ❌ = no aplica

---

## 🗳️ Plantilla de decisión

Rellenar entre todos antes de cerrar la idea:

| Pregunta | Respuesta del equipo |
|----------|----------------------|
| ¿Qué idea nos llama más la atención? | |
| ¿Qué idea se ajusta mejor a las asignaturas? | |
| ¿Tenemos tiempo suficiente para la más compleja? | |
| ¿Alguien del equipo ya domina alguna tecnología clave? | |
| ¿Qué idea nos motiva para trabajar meses en ella? | |

**Idea elegida:** _(pendiente)_

**Justificación:** _(pendiente)_

---

## 📅 Próximos pasos

1. Leer este README en grupo.
2. Votar la idea (cada miembro elige 2 y se suman puntos).
3. Rellenar la plantilla de decisión.
4. Esbozar entidades, endpoints y pantallas de la idea elegida.
5. Repartir roles y crear issues en el repositorio.

---

## 📝 Notas

- Las ideas son **propuestas**, no definitivas: se pueden mezclar funcionalidades.
- Cualquier idea debe cumplir los **requisitos mínimos** indicados arriba.
- Este README se actualizará cuando se decida la idea final.

---