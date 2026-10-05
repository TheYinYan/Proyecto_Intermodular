# 🎓 Proyecto Intermodular 2DAM — Trukko

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

## 🛒 "Trukko": Trueque de Objetos

**Descripción:**
Plataforma donde los usuarios publican objetos que ya no usan (libros, apuntes, componentes, periféricos) y otros pueden solicitar un intercambio. El dueño acepta o rechaza la solicitud.

### **Funcionalidades clave:**
- Registro y login.
- Publicación de objetos con imagen, descripción y estado.
- Sistema de solicitudes con estados: pendiente / aceptada / rechazada.
- Historial de intercambios.

### **Tecnologías previstas:**
- Backend: (...).
- Base de datos: (...).
- Frontend: Angular o JS/TS.
- Subida de imágenes (...).

### **Asignaturas que cubre:**
- Acceso a Datos (transacciones, estados).
- Desarrollo de Interfaces (listados, detalle, formularios con imagen).
- Programación de Servicios (tareas programadas con hilos).
- Sistemas de Gestión Empresarial (flujo de negocio con reglas).
- Programación (backend Java).

### **Puntos fuertes:**
- Lógica de negocio real (no es un CRUD plano).
- Muy presentable en la defensa.
- Tarea programada → toca Programación de Servicios.

**Riesgos:**
- Más complejo de modelar (estados, permisos).

### **Ideas Planteadas**

#### **1. Uso IA**
- Que la IA le de un valor estimado para luego buscar productos de un valor similar
