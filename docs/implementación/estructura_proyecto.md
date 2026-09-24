---
sidebar_position: 1
---

# Estructura del Proyecto

El código fuente está organizado separando la lógica del programa, las interfaces gráficas y las consultas a la base de datos.

```text
OtakuTrack/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/otakutrack/
│   │   │       ├── model/          # Clases Java (Anime, Manga, Obra)
│   │   │       ├── view/           # Archivos FXML para la interfaz JavaFX
│   │   │       ├── controller/     # Controladores (Eventos de botones, tablas)
│   │   │       └── dao/            # Conexión JDBC (Data Access Object)
│   │   └── resources/
│   │       ├── css/                # Hojas de estilo para la aplicación
│   │       └── db/                 # Script SQL (creacion_tablas.sql)
├── README.md                       # Documentación inicial del repositorio
└── .gitignore                      # Archivos excluidos de Git
