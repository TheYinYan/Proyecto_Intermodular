# 🎓 Proyecto Intermodular 2DAM — MeteoLook

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

## 👕 "MeteoLook": Armario Virtual con Recomendaciones

**Descripción:**
Aplicación web/móvil donde el usuario sube fotos de su ropa, la etiqueta (tipo, color, temporada, ocasión) y la app le sugiere combinaciones de conjuntos según el clima del día (consumiendo una API meteorológica) y la ocasión (formal, casual, deporte). Además, permite registrar si el usuario se puso el conjunto sugerido, subiendo una foto, para ir aprendiendo de sus preferencias.

### **Diseño en Móvil**

![imagen](/Img/MeteoLookM.png)

> Pantallas incluidas: Carga, Registro, Inicio, Creación de prenda, Mi Ropero y Tiempo.

### **Diseño en Web**

![imagen](/Web-MeteoLook.png)

> _(Pendiente de subir el diseño web definitivo)_

---

### **Funcionalidades clave:**

- **Registro y login** de usuarios (con opción de "Iniciar sin ropero" para probar la app).
- **Pantalla de carga** con logo animado.
- **Pantalla de inicio** con:
  - Saludo personalizado ("Hola Samuel...").
  - Conjunto del día (imagen + descripción de por qué se ha elegido).
  - Estado del clima actual.
  - Botón "Otra combinación".
  - Botón "¿Ya te lo pusiste? Súbete una foto" para registrar el conjunto usado.
- **Pantalla de creación de prenda**:
  - Subir foto desde galería o hacer foto con la cámara.
  - Selección de tipo, color, temporada y ocasión.
  - Campo de notas.
  - Botón "Guardar prenda".
- **Pantalla "Mi Ropero"**:
  - Listado de prendas con imagen, tipo y color.
  - Buscador por texto.
  - Filtros por tipo, color, temporada y ocasión.
  - Botón "Añadir prenda".
- **Pantalla de Tiempo**:
  - Clima actual: temperatura, estado, ciudad, humedad, viento, sensación térmica.
  - Próximos días (previsión).
  - Sugerencia de conjunto para hoy ("Ver conjunto").
  - Frase del día relacionada con el clima.
- **Algoritmo de recomendación** basado en reglas:
  - Si llueve → incluir paraguas y calzado adecuado.
  - Si hace frío → abrigo, jersey, etc.
  - Si hace calor → ropa ligera.
  - Según ocasión → formal, casual, deporte.
- **Consumo de API meteorológica** (OpenWeather o similar).
- **Subida de imágenes** (multipart) para prendas y conjuntos usados.

---

### **Tecnologías previstas:**

- Backend: Java + Spring Boot + HttpClient (para API del clima).
- Base de datos: MySQL / PostgreSQL (usuarios, prendas, conjuntos, historial).
- Frontend: Angular o JS/TS.
- Subida de imágenes (multipart) y almacenamiento local o en la nube.
- API externa: OpenWeather (o similar).

> _(Completar cuando se decida el stack definitivo)_

---

### **Asignaturas que cubre:**

- **Acceso a Datos** → relaciones usuario-prenda-conjunto, consultas, filtros, imágenes.
- **Desarrollo de Interfaces** → pantallas de ropero, creación, inicio, clima; filtros visuales; subida de imágenes.
- **Programación de Servicios y Procesos** → API REST propia + consumo de API externa (clima).
- **Sistemas de Gestión Empresarial** → lógica de recomendación, estados del conjunto, historial.
- **Programación** → backend Java con buenas prácticas.

---

### **Puntos fuertes:**

- Idea original y cotidiana.
- El "algoritmo de recomendación" suena muy bien en la defensa, aunque sea simple (reglas).
- API externa → cubre Programación de Servicios.
- Subida de imágenes → cubre Desarrollo de Interfaces y Acceso a Datos.
- Muy visual y fácil de demostrar en vivo.

---

### **Riesgos:**

- Subida y gestión de imágenes añade complejidad (almacenamiento, formatos, peso).
- Dependencia de una API externa (hay que manejar errores y límites de peticiones).
- El algoritmo de recomendación puede volverse complejo si se quiere hacer "inteligente" de verdad.

---

### **Ideas Planteadas**

#### **1. Uso de IA**
- Que la IA sugiera combinaciones según el clima, la ocasión y el historial del usuario.
- Que la IA ayude a etiquetar automáticamente las prendas al subir la foto (tipo, color, temporada).
- Que la IA genere una descripción del porqué de la combinación elegida.

#### **2. Secciones**
- **Mi Ropero** → gestión de prendas.
- **Conjunto del día** → recomendación diaria.
- **Historial** → conjuntos usados y valoraciones.
- **Tiempo** → clima actual y previsión.
- **Perfil** → datos del usuario, preferencias, ocasiones habituales.

#### **3. Extras posibles**
- Modo "compartir conjunto" en redes.
- Estadísticas de uso (prendas más usadas, colores favoritos).
- Notificación diaria con el conjunto sugerido.
- Integración con calendario para saber la ocasión del día (trabajo, clase, evento).

---

## 📅 Próximos pasos

1. Validar el diseño de pantallas (móvil y web) con el equipo.
2. Decidir el stack definitivo (backend, frontend, base de datos, API del clima).
3. Esbozar el modelo de datos (usuarios, prendas, conjuntos, historial).
4. Definir los endpoints de la API REST.
5. Repartir tareas por asignatura y crear issues en el repositorio.

---

[Ver Idea 1](../Readme.md)

> ⭐ "Si esperas el sol, no llega; si sales con paraguas, escampa." ⭐