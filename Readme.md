# 🎓 Proyecto Intermodular 2DAM — Trukko

> Repositorio de trabajo para la elección, planificación y desarrollo del Proyecto Intermodular de 2DAM.

---

## 👥 Equipo

| Nombre   | Rol propuesto     | GitHub |
|----------|-------------------|--------|
| Samuel   | Programador/Líder | [Enlace](https://github.com/TheYinYan) |
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
Plataforma donde los usuarios publican objetos que ya no usan (libros, apuntes, componentes, periféricos, servicios, tareas) y otros pueden solicitar un intercambio. El dueño acepta o rechaza la solicitud. La app incluye un sistema de favoritos y mensajería interna para gestionar los trueques.

---

### **Diseño en Móvil**

![imagen](/Img/Movil.png)

> **Pantallas diseñadas:**
>
> 1. **Pantalla de Carga:** Logo de Trukko con icono animado y texto "Cargando...".
> 2. **Pantalla de Registro:** Formulario de usuario y contraseña, botón "Iniciar sesión" y opción "Iniciar sin Ropero".
> 3. **Pantalla de Inicio:**
>    - Barra superior: menú hamburguesa, logo "Trukko", icono de perfil "Tu Cuenta".
>    - Barra de navegación horizontal: Inicio, Favoritos, Subir, Mensaje.
>    - Buscador y rejilla de 2 columnas con tarjetas (imagen, icono de perfil, corazón de favorito).
>    - Barra inferior con 5 iconos: Inicio, Favoritos, Subir (+), Mensajes, Perfil.
> 4. **Pantalla de Inicio con desplazamiento:** Similar a la anterior, con buscador expandido y rejilla más grande.
> 5. **Pantalla de Creación (Crear Objeto):**
>    - Vista previa de foto, botones "Subir foto" y "Tomar foto".
>    - Formulario: Título, Descripción, Categoría (Select), Estado (Select), Valor aprox. (€).
>    - Botón "Crear objeto".
> 6. **Pantalla de Mis Objetos:**
>    - Título "Mis objetos (12)".
>    - Buscador, filtros: [Todos] [Objetos] [Servicios] [Tareas] [Recientes].
>    - Rejilla de tarjetas con imagen, botón "Editar" y corazón.
>    - Botón "Crear un objeto".
> 7. **Pantalla de Favoritos:**
>    - Título "Mis Favoritos (8)".
>    - Buscador, filtros: [Todos] [Objetos] [Servicios] [Tareas] [Recientes].
>    - Rejilla de tarjetas con imagen, título y corazón relleno (❤️).
>    - Botón "Crear un objeto".
> 8. **Pantalla de Perfil (Ajuste de Perfil):**
>    - Foto de perfil con botones "Subir foto" y "Tomar foto".
>    - Botón "Editar Perfil".
>    - Nombre Usuario: Samuel, ⭐ 4.8 (23 valoraciones), Ubicación: 📍 Madrid.
>    - Opciones: Mis objetos (12), Mis Favoritos (8), Mensajes (5), Cerrar sesión.
> 9. **Pantalla de Mensajes (Lista de Chats):**
>    - Título "Mensajes (5)".
>    - Buscador de conversaciones.
>    - Lista de chats con: Usuario, Hora, Último Mensaje, Objeto a intercambiar, y badge rojo de no leídos.
>    - Ejemplos: Mari Paz (12:30, "¿Te interesa el libro?", Libro de Java), Carlos (11:15, "Te lo cambio por...", Auriculares), Luis Díaz (Ayer, "¿Tienes el Curso Java?", Manual TypeScript).
> 10. **Pantalla de Chat Individual:**
>     - Barra superior: "Usuario" y "Objeto a intercambiar".
>     - Tarjeta del objeto ofrecido con botón "Ver Objeto".
>     - Burbujas de mensaje (izquierda: otro usuario, derecha: tú).
>     - Campo de texto "Escribe un mensaje..." con icono de enviar.
>     - Barra inferior con el icono de Mensajes activo.

---

### **Diseño en Web**

![imagen](/Img/Web.png)

> **Pantallas diseñadas:**
>
> 1. **Pantalla de Login:** Interfaz centrada con el logo de Trukko, campos de "Usuario" y "Contraseña", botón "Iniciar sesión" y opción "Iniciar sin Ropero".
> 2. **Pantalla de Inicio (Web):**
>    - Barra superior: menú hamburguesa, logo de Trukko centrado, icono de perfil "Tu Cuenta".
>    - Barra de navegación horizontal: Inicio, Favoritos, Subir, Mensaje.
>    - Buscador y rejilla de 4 columnas con tarjetas (imagen, icono de perfil, corazón de favorito).
>    - Barra inferior con 5 iconos: Inicio, Favoritos, Subir (+), Mensajes, Perfil.
> 3. **Pantalla de Creación (Crear Objeto):** Similar a la móvil, pero adaptada a escritorio.
> 4. **Pantalla de Mis Objetos:** Similar a la móvil, con rejilla más amplia.
> 5. **Pantalla de Favoritos:** Similar a la móvil, con rejilla más amplia.
> 6. **Pantalla de Ajuste de Perfil:** Similar a la móvil, adaptada a escritorio.
> 7. **Pantalla de Mensajes (Lista de Chats):** Similar a la móvil, con más espacio.
> 8. **Pantalla de Chat Individual:** Similar a la móvil, adaptada a escritorio.

---

### **Funcionalidades clave:**

- **Registro y login** de usuarios (con opción de "Iniciar sin Ropero").
- **Publicación de objetos** con imagen, título, descripción, categoría, estado y valor aproximado.
- **Sistema de solicitudes** con estados: pendiente / aceptada / rechazada.
- **Historial de intercambios** y valoraciones.
- **Sistema de favoritos** (corazón relleno/vacío).
- **Mensajería interna** entre usuarios para negociar el trueque.
- **Búsqueda y filtros** por categoría (Objetos, Servicios, Tareas) y recientes.
- **Perfil de usuario** con objetos publicados, favoritos, mensajes e historial.
- **Subida de imágenes** para los objetos publicados.

---

### **Tecnologías previstas:**

- **Backend:** Java + Spring Boot (API REST).
- **Base de datos:** MySQL / PostgreSQL (usuarios, objetos, solicitudes, mensajes, favoritos).
- **Frontend:** Angular o JS/TS.
- **Subida de imágenes:** Multipart (almacenamiento local o en la nube).
- **Mensajería:** WebSockets o polling para mensajes en tiempo real (opcional).

---

### **Asignaturas que cubre:**

- **Acceso a Datos** → relaciones usuario-objeto-solicitud-mensaje, transacciones, estados, historial.
- **Desarrollo de Interfaces** → listados, detalle, formularios con imagen, sistema de favoritos, mensajería, navegación móvil/web.
- **Programación de Servicios y Procesos** → API REST, tareas programadas (caducidad de solicitudes), mensajería (hilos/WebSockets).
- **Sistemas de Gestión Empresarial** → flujo de negocio con reglas (estados de solicitud), roles, permisos.
- **Programación** → backend Java con buenas prácticas.

---

### **Puntos fuertes:**

- **Lógica de negocio real** (no es un CRUD plano): estados, solicitudes, mensajería, favoritos.
- **Muy presentable en la defensa** gracias a los diseños móviles y web ya creados.
- **Tarea programada** → cubre Programación de Servicios.
- **Mensajería interna** → añade complejidad y valor al proyecto.
- **Sistema de favoritos** → mejora la experiencia de usuario y la interactividad.
- **Diseño responsive** → la misma app se adapta a móvil y web.

---

### **Riesgos:**

- **Más complejo de modelar** (estados, permisos, mensajería).
- **Subida y gestión de imágenes** añade complejidad.
- **Mensajería en tiempo real** puede requerir WebSockets o polling.
- **Adaptación responsive** → asegurar que funciona en ambos formatos.

---

### **Ideas Planteadas**

#### **1. Uso IA**
- Que la IA le dé un **valor estimado** a los objetos para luego buscar productos de un valor similar.
- **Ayuda en la creación** de un nuevo producto: sugerir categoría, descripción o valoración basada en la imagen.
- **Recomendaciones personalizadas** de objetos según el historial del usuario.

#### **2. Secciones**
- **Intercambio de Tareas** → usuarios ofrecen realizar tareas a cambio de otras.
- **Intercambio de Servicios** → usuarios ofrecen servicios (clases, reparaciones) a cambio de otros.
- **Intercambio de Objetos Variados** → libros, apuntes, componentes, periféricos, etc.

#### **3. Extras posibles**
- **Modo "trueque rápido"** con coincidencia automática entre usuarios.
- **Estadísticas** de trueques realizados, objetos más solicitados, etc.
- **Notificaciones push** para nuevas solicitudes o mensajes.
- **Integración con calendario** para tareas o servicios con fecha.

---

## 📅 Próximos pasos

1. **Validar el diseño de pantallas** (móvil y web) con el equipo.
2. **Decidir el stack definitivo** (backend, frontend, base de datos, mensajería).
3. **Esbozar el modelo de datos** (usuarios, objetos, solicitudes, mensajes, favoritos).
4. **Definir los endpoints de la API REST** (ej: `/api/objetos`, `/api/solicitudes`, `/api/mensajes`).
5. **Repartir tareas por asignatura** y crear issues en el repositorio.

---

[Ver Idea 2 - MeteoLook](/MeteoLook/Readme.md)

[Ver Idea 3 - Plataforma de transicion profesional](/Plataforma%20de%20transicion%20profesional/Readme.md)