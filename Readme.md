# 🎓 Proyecto Intermodular 2DAM — Lookeo

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

## 👕 "Lookeo": Armario Virtual con Probador IA

**Descripción:**
Aplicación web/móvil donde el usuario sube fotos de su ropa, la etiqueta (tipo, color, temporada, ocasión) y la app le sugiere combinaciones de conjuntos. Además, incluye un **probador virtual con IA** que muestra cómo le queda la ropa al usuario, y permite guardar los conjuntos en la sección **Outfits**.

**Paleta de colores:**
- **Negro** (#000000) → fondo principal.
- **Dorado** (#D4AF37) → acentos, botones, logo.
- **Blanco** (#FFFFFF) → textos y elementos secundarios.

**Estilos de moda que promueve:**
- **Old Money / Elegante clásico:** blazers, camisas, pantalones de vestir, mocasines.
- **Streetwear de lujo:** sudaderas oversize, zapatillas de diseño, chaquetas bomber.
- **Minimalista / Clean:** básicos, colores neutros, líneas simples.

---

### [**Diseños**](/page/Diseño.md)

### **Funcionalidades clave:**

- **Registro y login** de usuarios.
- **Subida de prendas** con imagen, tipo, color, temporada y ocasión.
- **Ropero personal** con buscador y filtros.
- **Probador virtual con IA:**
  - El usuario sube una foto suya de cuerpo entero.
  - La IA superpone las prendas seleccionadas sobre su cuerpo.
  - Genera una imagen realista del conjunto puesto.
  - Selector de estilo (Casual, Formal, Urbano, Deportivo, Elegante, Streetwear).
  - Botón "Otra combinación" para regenerar.
- **Outfits:** guardar conjuntos favoritos con nombre y prendas.
- **Perfil de usuario** con sus prendas, outfits e historial.
- **Subida de imágenes** (multipart) para prendas y fotos del usuario.

---

### **Tecnologías previstas:**

- **Backend:** (...).
- **Base de datos:** (...).
- **Frontend:** Angular o JS/TS.
- **Subida de imágenes:** Multipart (almacenamiento local o en la nube).
- **IA para probador virtual:**
  - **Opción A (simple):** remove.bg + OpenCV para superponer prendas.
  - **Opción B (avanzada):** IDM-VTON, OOTDiffusion o CatVTON vía Hugging Face.
- **IA generativa de imágenes:** Pollinations.ai, Black Forest Labs (FLUX) o Segmind.

---

### **Asignaturas que cubre:**

- **Acceso a Datos** → relaciones usuario-prenda-outfit, consultas, filtros, imágenes.
- **Desarrollo de Interfaces** → pantallas de ropero, creación, probador, outfits; filtros visuales; subida de imágenes.
- **Programación de Servicios y Procesos** → API REST propia + consumo de API externa (IA).
- **Sistemas de Gestión Empresarial** → lógica de recomendación, estilos, historial.
- **Programación** → backend Java con buenas prácticas.

---

### **Puntos fuertes:**

- **Idea original y diferencial:** el probador virtual con IA es un gran atractivo.
- **Paleta de colores elegante:** negro + dorado transmite premium.
- **Estilos de moda definidos:** Old Money + Streetwear de lujo.
- **IA integrada:** cubre Programación de Servicios y da valor añadido.
- **Subida de imágenes:** cubre Desarrollo de Interfaces y Acceso a Datos.
- **Muy visual y fácil de demostrar en vivo.**
- **Diseño responsive:** la misma app se adapta a móvil y web.

---

### **Riesgos:**

- **Integración de IA para probador virtual:** puede ser compleja y consumir recursos.
- **Subida y gestión de imágenes:** almacenamiento, formatos, peso.
- **Dependencia de APIs externas:** manejar errores y límites de peticiones.
- **Adaptación responsive:** asegurar que funciona en ambos formatos.

---

### **Ideas Planteadas**

#### **1. Uso de IA**
- **Probador virtual:** superponer prendas sobre la foto del usuario.
- **Etiquetado automático:** al subir una prenda, la IA sugiere tipo, color y temporada.
- **Recomendaciones personalizadas:** según el historial, los estilos preferidos y eltiempo de ese dia.
- **Generación de outfits:** la IA crea combinaciones nuevas a partir del ropero.

#### **2. Secciones**
- **Conjunto del día:** recomendación diaria basada en el clima y la ocasión.
- **Probador:** ver cómo te queda la ropa con IA.
- **Ropero:** gestionar todas tus prendas.
- **Outfits:** guardar y gestionar conjuntos favoritos.
- **Perfil:** datos del usuario, preferencias, historial.

#### **3. Extras posibles**
- **Modo "compartir outfit"** en redes sociales.
- **Estadísticas de uso:** prendas más usadas, colores favoritos.
- **Notificación diaria** con el conjunto sugerido.
- **Integración con calendario** para saber la ocasión del día.

---

## 📅 Próximos pasos

1. **Validar el diseño de pantallas** (móvil y web) con el equipo.
2. **Decidir el stack definitivo** (backend, frontend, base de datos, IA).
3. **Esbozar el modelo de datos** (usuarios, prendas, outfits, historial).
4. **Definir los endpoints de la API REST** (ej: `/api/prendas`, `/api/outfits`, `/api/probador`).
5. **Repartir tareas por asignatura** y crear issues en el repositorio.

---

## 🗄️ Modelo de datos orientativo

| Entidad | Campos principales |
|---------|--------------------|
| **Usuario** | id, nombre, email, contraseña, foto_perfil, ubicacion |
| **Prenda** | id, usuario_id, imagen, tipo, color, temporada, ocasion, notas |
| **Outfit** | id, usuario_id, nombre, imagen, fecha_creacion |
| **Outfit_Prenda** | outfit_id, prenda_id |
| **Probador** | id, usuario_id, foto_usuario, outfit_id, imagen_generada, fecha |
| **Favorito** | id, usuario_id, prenda_id |

---

## 🔗 Endpoints orientativos

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| `POST` | `/api/auth/register` | Registro de usuario. |
| `POST` | `/api/auth/login` | Login. |
| `GET` | `/api/prendas` | Listar prendas del usuario. |
| `POST` | `/api/prendas` | Subir nueva prenda. |
| `PUT` | `/api/prendas/{id}` | Editar prenda. |
| `DELETE` | `/api/prendas/{id}` | Eliminar prenda. |
| `GET` | `/api/outfits` | Listar outfits. |
| `POST` | `/api/outfits` | Crear outfit. |
| `POST` | `/api/probador` | Generar imagen con IA. |
| `GET` | `/api/probador/{id}` | Obtener resultado. |

---
