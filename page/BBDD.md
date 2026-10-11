[< Back](../Readme.md)

## 🗄️ Modelo de Datos — Lookeo

---

### 📐 Modelo Conceptual (E/R)

![DER Lookeo](/assets/Img/DER.png)
![DR Lookeo](/assets/Img/DR.png)

#### Entidades y atributos propios

| Entidad    | Atributos propios                                           | Descripción                             |
| ---------- | ----------------------------------------------------------- | --------------------------------------- |
| _Usuario_  | id_usuario, nombre, email, password, foto_perfil, ubicacion | Usuario registrado en la app.           |
| _Prenda_   | id_prenda, imagen, tipo, color, estilo, temporada, notas    | Prenda del ropero del usuario.          |
| _Outfit_   | id_outfit, nombre, imagen, fecha_creacion                   | Conjunto de prendas guardado.           |
| _Probador_ | id_probador, foto_usuario, img_generada, fecha              | Resultado de una prueba virtual con IA. |

> _Nota:_ En el modelo conceptual, id*usuario \_no aparece* en Prenda, Outfit ni Probador, porque las relaciones ya lo representan.

#### Relaciones

| Relación          | Cardinalidad | Descripción                                                                |
| ----------------- | ------------ | -------------------------------------------------------------------------- |
| Usuario → Prenda  | 1:N          | Un usuario tiene muchas prendas.                                           |
| Usuario → Outfit  | 1:N          | Un usuario tiene muchos outfits.                                           |
| Outfit ↔️ Prenda  | N:M          | Un outfit tiene muchas prendas y una prenda puede estar en varios outfits. |
| Outfit → Probador | 1:N          | Un outfit puede generar muchas pruebas virtuales.                          |

---

### 💻 Modelo Relacional (SQL)

En la implementación, las relaciones se convierten en _claves foráneas_.

#### Claves foráneas

| Tabla           | Clave foránea         | Referencia      |
| --------------- | --------------------- | --------------- |
| _Prenda_        | id_usuario            | Usuario         |
| _Outfit_        | id_usuario            | Usuario         |
| _Outfit_Prenda_ | id_outfit, id_prenda  | Outfit, Prenda  |
| _Probador_      | id_outfit, id_usuario | Outfit, Usuario |

#### Script SQL

```sql
CREATE TABLE usuario (
  id_usuario INT PRIMARY KEY AUTO_INCREMENT,
  nombre VARCHAR(100) NOT NULL,
  email VARCHAR(150) UNIQUE NOT NULL,
  password VARCHAR(255) NOT NULL,
  foto_perfil VARCHAR(255),
  ubicacion VARCHAR(100)
);

CREATE TABLE prenda (
  id_prenda INT PRIMARY KEY AUTO_INCREMENT,
  id_usuario INT NOT NULL,
  imagen VARCHAR(255),
  tipo VARCHAR(50),
  color VARCHAR(50),
  estilo VARCHAR(50),
  temporada VARCHAR(50),
  notas TEXT,
  FOREIGN KEY (id_usuario) REFERENCES usuario(id_usuario)
);

CREATE TABLE outfit (
  id_outfit INT PRIMARY KEY AUTO_INCREMENT,
  id_usuario INT NOT NULL,
  nombre VARCHAR(100),
  imagen VARCHAR(255),
  fecha_creacion DATETIME DEFAULT CURRENT_TIMESTAMP,
  FOREIGN KEY (id_usuario) REFERENCES usuario(id_usuario)
);

CREATE TABLE outfit_prenda (
  id_outfit INT,
  id_prenda INT,
  PRIMARY KEY (id_outfit, id_prenda),
  FOREIGN KEY (id_outfit) REFERENCES outfit(id_outfit),
  FOREIGN KEY (id_prenda) REFERENCES prenda(id_prenda)
);

CREATE TABLE probador (
  id_probador INT PRIMARY KEY AUTO_INCREMENT,
  id_outfit INT NOT NULL,
  id_usuario INT NOT NULL,
  foto_usuario VARCHAR(255),
  img_generada VARCHAR(255),
  fecha DATETIME DEFAULT CURRENT_TIMESTAMP,
  FOREIGN KEY (id_outfit) REFERENCES outfit(id_outfit),
  FOREIGN KEY (id_usuario) REFERENCES usuario(id_usuario)
);
```
