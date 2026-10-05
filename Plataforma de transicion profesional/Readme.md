# 🎓 Proyecto Intermodular 2DAM — Plataforma de Transición Profesional

> Repositorio de trabajo para la elección, planificación y desarrollo del Proyecto Intermodular de 2DAM.

---

## 👥 Equipo

| Nombre   | Rol propuesto     | GitHub                                 |
| -------- | ----------------- | -------------------------------------- |
| Samuel   | Programador/Líder | [Enlace](https://github.com/TheYinYan) |
| Mari Paz | Programador       | [Enlace](https://github.com/mpjmar)    |

> Los roles son orientativos y pueden rotarse durante el proyecto.

---

## 🎯 Objetivo del Proyecto Intermodular

Diseñar y desarrollar una plataforma que ayude a personas que quieren **cambiar de profesión sin tener que empezar desde cero**, identificando las competencias adquiridas durante su trayectoria profesional y relacionándolas con nuevas oportunidades laborales.

La aplicación analizará la experiencia y conocimientos del usuario para construir un recorrido personalizado:

> **Lo que ya sabes → Profesiones posibles → Qué te falta → Cómo formarte → Dónde puedes trabajar**

El proyecto permitirá integrar los conocimientos adquiridos en las diferentes asignaturas del ciclo:

- **Acceso a Datos** → base de datos relacional, relaciones, consultas y gestión de información.
- **Desarrollo de Interfaces** → frontend, formularios, perfiles, resultados y navegación.
- **Programación de Servicios y Procesos** → API REST, consumo de servicios externos y tareas programadas.
- **Sistemas de Gestión Empresarial** → usuarios, roles, procesos y lógica de negocio.
- **Programación** → desarrollo del backend en Java y aplicación de buenas prácticas.

### Requisitos mínimos

- Backend desarrollado en **Java + Spring Boot**.
- API **REST**.
- Base de datos **relacional**: MySQL / PostgreSQL.
- Frontend que consuma la API: **Angular / TypeScript**.
- Sistema de autenticación.
- Gestión de perfiles y competencias.
- Al menos una funcionalidad avanzada:
  - consumo de API externa,
  - tareas programadas,
  - roles y permisos,
  - integración con servicios de IA.

---

# 💼 Plataforma de Transición Profesional

## 📝 Descripción

La plataforma está dirigida a personas que quieren **reorientar su carrera profesional**, especialmente aquellas que consideran que para cambiar de profesión tienen que empezar prácticamente desde cero.

El sistema parte de una idea fundamental:

> **La experiencia profesional acumulada también tiene valor en una nueva profesión.**

En lugar de limitarse a mostrar ofertas de empleo, la aplicación analizará las **competencias, conocimientos y experiencia** de una persona para detectar posibles caminos profesionales.

Por ejemplo, una persona con muchos años de experiencia en administración podría descubrir que parte de sus competencias son transferibles a puestos relacionados con:

- Gestión digital.
- Soporte de aplicaciones.
- Gestión de proyectos.
- Atención y soporte técnico.
- Gestión de sistemas de información.
- Otras profesiones relacionadas.

El objetivo es mostrar al usuario **qué puede aprovechar de su experiencia actual y qué necesita aprender para acceder a una nueva profesión**.

---

## 🔄 Funcionamiento general

El recorrido principal de la aplicación será:

```text
Experiencia profesional
        ↓
Competencias adquiridas
        ↓
Análisis del perfil
        ↓
Profesiones compatibles
        ↓
Competencias que faltan
        ↓
Formación recomendada
        ↓
Ofertas de empleo
        ↓
Empresas
```

La aplicación no pretende decir al usuario:

> "Tu profesión es X."

Sino ofrecerle diferentes posibilidades:

> "Con tu experiencia actual, estas son algunas profesiones a las que podrías acceder y estos son los conocimientos que necesitarías adquirir."

---

# 👤 Perfil del usuario

El usuario podrá crear un perfil profesional indicando, entre otros datos:

- Experiencia laboral.
- Puestos desempeñados.
- Años de experiencia.
- Formación.
- Conocimientos técnicos.
- Competencias profesionales.
- Competencias personales.
- Idiomas.
- Intereses profesionales.

La información podrá introducirse manualmente y, en una fase posterior, mediante herramientas que faciliten la creación del perfil.

### Ejemplo

```text
Experiencia:
Administración — 15 años

Competencias:
- Gestión documental
- Atención al cliente
- Organización
- Gestión de información
- Trabajo con herramientas ofimáticas
- Resolución de problemas
```

A partir de esta información, el sistema podrá identificar posibles competencias transferibles.

---

# 🧭 Exploración de profesiones

La plataforma mostrará diferentes profesiones que podrían ser accesibles para el usuario.

Cada profesión tendrá información como:

- Descripción.
- Competencias necesarias.
- Competencias que ya posee el usuario.
- Competencias que necesita adquirir.
- Formación relacionada.
- Nivel de compatibilidad.
- Ofertas de empleo relacionadas.

### Ejemplo

```text
GESTIÓN DE PROYECTOS
────────────────────────────

Compatibilidad: 72 %

✓ Organización
✓ Gestión documental
✓ Atención a clientes
✓ Coordinación

Necesitas desarrollar:

○ Metodologías ágiles
○ Herramientas de gestión de proyectos
○ Gestión de equipos

Formación recomendada:
→ Curso de Scrum
→ Jira / Trello
→ Gestión de proyectos
```

---

# 🤖 Inteligencia Artificial

La IA será una funcionalidad complementaria de la plataforma.

Su objetivo no será sustituir el análisis del sistema, sino **ayudar a interpretar información profesional y laboral**.

### Posibles usos

**1. Análisis del perfil**

La IA podrá analizar la experiencia introducida por el usuario para detectar posibles competencias.

**2. Identificación de competencias transferibles**

Podrá relacionar experiencias profesionales con competencias utilizadas en otras profesiones.

**3. Análisis de ofertas de empleo**

La aplicación podrá analizar ofertas reales para detectar:

- Tecnologías demandadas.
- Competencias.
- Formación requerida.
- Experiencia.
- Idiomas.

**4. Recomendaciones**

A partir de las diferencias entre el perfil del usuario y una profesión determinada, la IA podrá ayudar a generar recomendaciones de aprendizaje.

> La IA será una herramienta de apoyo. Las recomendaciones deberán poder ser interpretadas y justificadas por la aplicación.

---

# 📚 Formación

Una vez identificadas las competencias que faltan, la aplicación podrá mostrar diferentes opciones de formación.

Por ejemplo:

```text
Profesión objetivo:
Desarrollador Frontend

Competencias que faltan:

JavaScript       ███████░░░
TypeScript       █████░░░░░
Angular          ███░░░░░░░
Git              ████████░░

Formación recomendada:

→ TypeScript desde cero
→ Angular
→ Git y GitHub
→ Desarrollo de aplicaciones web
```

La formación podrá proceder de:

- Cursos.
- Centros de formación.
- Plataformas educativas.
- Recursos gratuitos.
- Certificaciones.

---

# 💼 Ofertas de empleo

La plataforma podrá incorporar ofertas de empleo obtenidas mediante una API externa o mediante otra fuente de datos.

Las ofertas podrán relacionarse con las profesiones y competencias de la plataforma.

Para cada oferta se podrá mostrar:

- Empresa.
- Puesto.
- Ubicación.
- Modalidad.
- Requisitos.
- Competencias solicitadas.
- Nivel de compatibilidad con el perfil del usuario.

### Ejemplo

```text
Desarrollador Junior Java

Compatibilidad: 68 %

✓ Java
✓ Git
✓ Bases de datos

Necesitas mejorar:

○ Spring Boot
○ APIs REST
```

---

# 🏢 Empresas

La plataforma también podrá contemplar un perfil específico para empresas.

Las empresas podrán:

- Crear un perfil.
- Publicar ofertas.
- Definir competencias necesarias.
- Buscar perfiles profesionales.
- Consultar candidatos compatibles.

Esto permitiría que la plataforma conectase los dos lados del mercado:

```text
PERSONAS                         EMPRESAS

Experiencia                      Puestos
     ↓                              ↓
Competencias       ←→          Competencias
     ↓                              ↓
Profesiones                       Ofertas
```

---

# 👥 Tipos de usuario

Inicialmente se contemplarán diferentes roles:

### 👤 Usuario

Puede:

- Crear y editar su perfil.
- Añadir experiencia.
- Gestionar sus competencias.
- Explorar profesiones.
- Consultar sus compatibilidades.
- Guardar profesiones.
- Consultar formación.
- Consultar ofertas.

### 🏢 Empresa

Puede:

- Gestionar su perfil.
- Publicar ofertas.
- Definir requisitos.
- Consultar candidatos compatibles.

### 👨‍💼 Administrador

Puede:

- Gestionar usuarios.
- Gestionar profesiones.
- Gestionar competencias.
- Gestionar categorías.
- Supervisar ofertas y contenidos.

---

# ⭐ Funcionalidades clave

- **Registro y login** de usuarios.
- **Creación de perfil profesional**.
- Gestión de experiencia laboral.
- Gestión de competencias.
- Identificación de competencias transferibles.
- Exploración de profesiones.
- Cálculo de compatibilidad entre perfil y profesión.
- Identificación de competencias que faltan.
- Recomendación de formación.
- Consulta de ofertas de empleo.
- Sistema de favoritos.
- Perfil de empresas.
- Publicación de ofertas.
- Roles y permisos.
- Integración con servicios externos.
- Uso de IA para análisis y recomendaciones.

---

# 🗄️ Modelo de datos inicial

Algunas de las entidades principales podrían ser:

```text
Usuario
   │
   ├── Experiencia
   │
   ├── Competencia
   │
   ├── Formación
   │
   └── Favoritos

Competencia
   │
   ├── Profesión
   │
   └── Oferta

Profesión
   │
   ├── Competencias
   ├── Formación
   └── Ofertas

Empresa
   │
   └── Oferta
```

### Entidades previstas

- Usuario
- Rol
- Experiencia
- Competencia
- Profesión
- Formación
- Empresa
- Oferta
- Favorito
- Recomendación

> El modelo definitivo se diseñará durante la fase de análisis.

---

# 🛠️ Tecnologías previstas

### Backend

- **Java**
- **Spring Boot**
- Spring Web
- Spring Data JPA
- Spring Security

### Base de datos

- **PostgreSQL** / MySQL
- JPA / Hibernate

### Frontend

- **Angular**
- TypeScript
- HTML
- CSS

### Servicios externos

Posibles integraciones:

- API de ofertas de empleo.
- API de formación.
- Servicio de IA.
- Otros servicios relacionados con el mercado laboral.

### Infraestructura

- Git / GitHub
- Docker
- Postman
- Maven

---

# 📚 Asignaturas que cubre

### Acceso a Datos

- Modelo relacional.
- Relaciones entre entidades.
- JPA / Hibernate.
- Consultas.
- Persistencia.
- Transacciones.

### Desarrollo de Interfaces

- Aplicación web.
- Componentes Angular.
- Formularios.
- Navegación.
- Perfiles.
- Visualización de competencias.
- Resultados y recomendaciones.

### Programación de Servicios y Procesos

- API REST.
- Consumo de APIs externas.
- Tareas programadas.
- Integración con servicios externos.
- Procesamiento de información.

### Sistemas de Gestión Empresarial

- Usuarios y roles.
- Empresas.
- Ofertas.
- Procesos de selección.
- Gestión de permisos.

### Programación

- Backend Java.
- Programación orientada a objetos.
- Arquitectura por capas.
- Validaciones.
- Excepciones.
- Buenas prácticas.

---

# 💪 Puntos fuertes

### 🎯 Problema real

La transformación tecnológica está provocando que muchas profesiones cambien y que determinadas competencias queden obsoletas o necesiten complementarse.

La plataforma aborda el problema desde una perspectiva diferente:

> **No empezar de cero, sino descubrir qué parte de tu experiencia sigue teniendo valor.**

### 🔄 Tiene recorrido

El proyecto puede comenzar con un sistema sencillo basado en competencias y evolucionar progresivamente hacia:

- IA.
- Análisis de ofertas.
- Recomendaciones.
- Empresas.
- Formación.
- Matching entre candidatos y ofertas.

### 🧠 Tiene lógica de negocio

No se trata únicamente de realizar un CRUD.

Existen procesos como:

```text
Perfil → Competencias → Profesión
                    ↓
              Compatibilidad
                    ↓
             Competencias faltantes
                    ↓
                Formación
                    ↓
                 Empleo
```

### 🎓 Permite integrar las asignaturas

El proyecto permite justificar de forma natural el uso de backend, base de datos, frontend, API REST, autenticación, servicios externos, roles e inteligencia artificial.

### 🚀 Potencial de ampliación

La aplicación podría evolucionar posteriormente hacia una plataforma dirigida también a:

- Empresas.
- Centros de formación.
- Servicios de empleo.
- Orientadores profesionales.

---

# ⚠️ Riesgos

### 🤖 Dependencia de la IA

La IA puede añadir complejidad y generar resultados poco consistentes.

**Solución:** comenzar con un sistema de competencias y reglas definido por el equipo y añadir IA progresivamente.

### 📊 Obtención de ofertas reales

Conseguir datos de ofertas de empleo mediante APIs puede ser complicado.

**Solución:** diseñar inicialmente la aplicación para trabajar con datos propios y posteriormente incorporar una API externa.

### 🧩 Complejidad del sistema de compatibilidad

Relacionar competencias con profesiones requiere un modelo de datos bien diseñado.

**Solución:** comenzar con un conjunto reducido de profesiones y competencias y ampliar progresivamente.

### 📈 Alcance excesivo

La idea puede crecer rápidamente.

**Solución:** definir un MVP antes de comenzar el desarrollo.

---

# 🚧 MVP propuesto

La primera versión funcional de la plataforma incluirá:

1. Registro y login.
2. Creación del perfil profesional.
3. Introducción de experiencia.
4. Gestión de competencias.
5. Catálogo de profesiones.
6. Relación profesión ↔ competencias.
7. Cálculo de compatibilidad.
8. Identificación de competencias faltantes.
9. Recomendación básica de formación.
10. Sistema de favoritos.

Una vez terminado el MVP se podrán incorporar:

- IA.
- Ofertas reales.
- Empresas.
- Matching candidato/oferta.
- Análisis automático de ofertas.
- Notificaciones.
- Estadísticas.

---

# 💡 Posibles ampliaciones

### 🤖 Análisis inteligente

La IA podría analizar una descripción como:

> "He trabajado durante 15 años atendiendo pacientes, gestionando citas, documentación y resolviendo problemas con usuarios."

Y transformarla en competencias estructuradas:

```text
✓ Atención al cliente
✓ Gestión documental
✓ Organización
✓ Gestión de incidencias
✓ Comunicación
✓ Trabajo bajo presión
```

### 🔎 "¿A qué puedo dedicarme?"

Una funcionalidad especialmente interesante sería permitir al usuario descubrir profesiones que quizá no conocía.

```text
Con tu experiencia podrías explorar:

1. Soporte de aplicaciones      82 %
2. Gestión de proyectos         76 %
3. Customer Success             73 %
4. Gestión digital              69 %
5. Soporte técnico              64 %
```

### ⚡ Brecha profesional

Mostrar de forma visual qué distancia existe entre el perfil actual y una profesión objetivo:

```text
PERFIL ACTUAL
      ↓
██████████████░░░░
      70 %
      ↓
PROFESIÓN OBJETIVO
```

Esto permitiría convertir el proceso de cambio profesional en un **itinerario concreto y comprensible**.

---

# 📅 Próximos pasos

1. **Definir el MVP** y limitar el alcance inicial.
2. Identificar las **entidades principales**.
3. Diseñar el **modelo de datos**.
4. Definir las relaciones entre **competencias y profesiones**.
5. Diseñar los primeros wireframes.
6. Decidir el stack definitivo.
7. Diseñar la arquitectura del backend.
8. Definir los endpoints de la API REST.
9. Crear el proyecto Angular.
10. Crear el proyecto Spring Boot.
11. Configurar la base de datos.
12. Repartir tareas entre los miembros del equipo.
13. Crear issues y milestones en GitHub.

---

## 🚀 Idea central

> **Cambiar de profesión no debería significar empezar desde cero.**
>
> La plataforma busca convertir la experiencia profesional de una persona en nuevas oportunidades, mostrando qué puede aprovechar, qué necesita aprender y cuál puede ser su siguiente paso profesional.

---

[Ver Idea 1](/Readme.md)

[Ver Idea 2](/MeteoLook/Readme.md)