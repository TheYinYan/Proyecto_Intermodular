# 🎓 Proyecto Intermodular 2DAM — Lookeo

> Repositorio de trabajo para la elección, planificación y desarrollo del Proyecto Intermodular de 2DAM.

---

## 👥 Equipo

| Nombre   | Rol            | GitHub                                     |
| -------- | -------------- | ------------------------------------------ |
| Samuel   | Desarrollador  | [@TheYinYan](https://github.com/TheYinYan) |
| Mari Paz | Desarrolladora | [@mpjmar](https://github.com/mpjmar)       |

> Los roles son orientativos y se pueden rotar durante el proyecto.

---

## 🎯 Objetivo del Proyecto Intermodular

Diseñar y desarrollar una aplicación completa que integre los conocimientos de las asignaturas del ciclo:

- _Acceso a Datos_ → base de datos real, relaciones, consultas.
- _Desarrollo de Interfaces_ → frontend funcional y usable.
- _Programación de Servicios y Procesos_ → API REST, tareas programadas, consumo de servicios externos.
- _Sistemas de Gestión Empresarial_ → lógica de negocio, roles, flujos.
- _Programación_ → backend en Node y Express con buenas prácticas.

_Requisitos mínimos que debe cumplir la idea elegida:_

- Backend en Node y Express con API REST.
- Base de datos _relacional_ (Supabase / PostgreSQL).
- Frontend que consuma la API (Angular, JS/TS, etc.).
- Autenticación de usuarios.
- Al menos _una_ de estas: consumo de API externa, tareas programadas, roles/permisos, subida de archivos.

---

## 👕 "Lookeo": Armario Virtual con Probador IA

### 🧩 Repositorios del proyecto

| Repo           | Descripción              | Enlace                                                       |
| -------------- | ------------------------ | ------------------------------------------------------------ |
| _Principal_    | Descripción del proyecto (este repo)| [Enlace](https://github.com/TheYinYan/Proyecto_Intermodular) |
| _Lookeo-Móvil_ | App móvil                | [Enlace](https://github.com/TheYinYan/Lookeo-Movil)          |
| _Lookeo-Web_   | App web                  | [Enlace](https://github.com/TheYinYan/Lookeo-Web)            |

#### [_> Diseños de la App y Web_](/page/Diseño.md)

_Descripción:_
Aplicación web/móvil donde el usuario sube fotos de su ropa, la etiqueta (tipo, color, temporada, ocasión) y la app le sugiere combinaciones de conjuntos. Además, incluye un _probador virtual con IA_ que muestra cómo le queda la ropa al usuario, y permite guardar los conjuntos en la sección _Outfits_.

_Paleta de colores:_

- _Negro_ (#000000) → fondo principal.
- _Dorado_ (#D4AF37) → acentos, botones, logo.
- _Blanco_ (#FFFFFF) → textos y elementos secundarios.

_Estilos de moda que promueve:_

- _Old Money / Elegante clásico:_ blazers, camisas, pantalones de vestir, mocasines.
- _Streetwear de lujo:_ sudaderas oversize, zapatillas de diseño, chaquetas bomber.
- _Minimalista / Clean:_ básicos, colores neutros, líneas simples.

---

### _Funcionalidades clave:_

- **_Registro y login_** de usuarios.
- **_Ropero personal_** con buscador y filtros.
- **_Subida de prendas_**: 
  - _En la App Móvil:_ Uso prioritario de la cámara y galería del dispositivo para agilizar el proceso de creación de ropa.
  - _En la Web:_ Subida de archivos desde el ordenador.
- **_Probador virtual con IA (Prioritario en Web):_**
  - El usuario sube una foto de cuerpo entero.
  - La IA superpone las prendas seleccionadas sobre su cuerpo generando una imagen realista.
  - Selector de estilo (Casual, Formal, Urbano, Deportivo, Elegante, Streetwear).
  - *Nota: Debido a la alta carga de procesamiento que requiere la IA, esta funcionalidad se ha centralizado en la versión Web. En la App Móvil se prioriza la visualización del conjunto del día y la gestión rápida del ropero.*
- **_Outfits:_** guardar conjuntos favoritos con nombre y prendas.
- **_Favoritos:_** sección para guardar prendas y looks preferidos (disponible en ambas).
- **_Perfil de usuario_** con sus prendas, outfits e historial.

---

### _Tecnologías previstas:_

- _Backend:_ En Node y Express con API REST.
- _Base de datos:_ Supabase / PostgreSQL.
- _Frontend:_ Angular o JS/TS.
- _Subida de imágenes:_ Multipart (almacenamiento local o en la nube).
- _IA para probador virtual:_
  - _Opción A (simple):_ remove.bg + OpenCV para superponer prendas.
  - _Opción B (avanzada):_ IDM-VTON, OOTDiffusion o CatVTON vía Hugging Face.
- _IA generativa de imágenes:_ Pollinations.ai, Black Forest Labs (FLUX) o Segmind.

---

### _Asignaturas que cubre:_

- _Acceso a Datos_ → relaciones usuario-prenda-outfit, consultas, filtros, imágenes.
- _Desarrollo de Interfaces_ → pantallas de ropero, creación, probador, outfits; filtros visuales; subida de imágenes.
- _Programación de Servicios y Procesos_ → API REST propia + consumo de API externa (IA).
- _Sistemas de Gestión Empresarial_ → lógica de recomendación, estilos, historial.
- _Programación_ → backend Node y Express con buenas prácticas.

---

### _Puntos fuertes:_

- _Idea original y diferencial:_ el probador virtual con IA es un gran atractivo.
- _Paleta de colores elegante:_ negro + dorado transmite premium.
- _Estilos de moda definidos:_ Old Money + Streetwear de lujo.
- _IA integrada:_ cubre Programación de Servicios y da valor añadido.
- _Subida de imágenes:_ cubre Desarrollo de Interfaces y Acceso a Datos.
- _Muy visual y fácil de demostrar en vivo._
- _Diseño responsive:_ la misma app se adapta a móvil y web.

---

### _Riesgos:_

- _Integración de IA para probador virtual:_ puede ser compleja y consumir recursos.
- _Subida y gestión de imágenes:_ almacenamiento, formatos, peso.
- _Dependencia de APIs externas:_ manejar errores y límites de peticiones.
- _Adaptación responsive:_ asegurar que funciona en ambos formatos.

---

### _Ideas Planteadas_

#### _1. Uso de IA_

- _Probador virtual:_ superponer prendas sobre la foto del usuario.
- _Etiquetado automático:_ al subir una prenda, la IA sugiere tipo, color y temporada.
- _Recomendaciones personalizadas:_ según el historial, los estilos preferidos y eltiempo de ese dia.
- _Generación de outfits:_ la IA crea combinaciones nuevas a partir del ropero.

#### _2. Secciones_

- _Conjunto del día:_ recomendación diaria basada en el clima y la ocasión.
- _Probador:_ ver cómo te queda la ropa con IA.
- _Ropero:_ gestionar todas tus prendas.
- _Outfits:_ guardar y gestionar conjuntos favoritos.
- _Perfil:_ datos del usuario, preferencias, historial.

#### _3. Extras posibles_

- _Modo "compartir outfit"_ en redes sociales.
- _Estadísticas de uso:_ prendas más usadas, colores favoritos.
- _Notificación diaria_ con el conjunto sugerido.
- _Integración con calendario_ para saber la ocasión del día.

---

## 🗄️ Modelo de Datos

📄 _[Ver modelo de datos completo](/page/BBDD.md)_

---

## 🔗 Endpoints orientativos

| Método | Endpoint           | Descripción                 |
| ------ | ------------------ | --------------------------- |
| POST   | /api/auth/register | Registro de usuario.        |
| POST   | /api/auth/login    | Login.                      |
| GET    | /api/prendas       | Listar prendas del usuario. |
| POST   | /api/prendas       | Subir nueva prenda.         |
| PUT    | /api/prendas/{id}  | Editar prenda.              |
| DELETE | /api/prendas/{id}  | Eliminar prenda.            |
| GET    | /api/outfits       | Listar outfits.             |
| POST   | /api/outfits       | Crear outfit.               |
| POST   | /api/probador      | Generar imagen con IA.      |
| GET    | /api/probador/{id} | Obtener resultado.          |

---

## 📅 Próximos pasos

1. _Validar el diseño de pantallas_ (móvil y web) con el equipo.
2. _Decidir el stack definitivo_ (backend, frontend, base de datos, IA).
3. _Esbozar el modelo de datos_ (usuarios, prendas, outfits, historial).
4. _Definir los endpoints de la API REST_ (ej: /api/prendas, /api/outfits, /api/probador).
5. _Repartir tareas por asignatura_ y crear issues en el repositorio.

---
