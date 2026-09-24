---
sidebar_position: 1
---

# Requisitos del Sistema

## Requisitos Funcionales

1. **Gestión de Entradas:** El usuario podrá añadir nuevas series de anime (ej. *Oshi no Ko*, *One Piece*) o manga (*Reincarnation no Kaben*) indicando título, autor/estudio, género y estado actual (viendo, completado, en pausa).
2. **Seguimiento de Progreso:** Se podrá actualizar dinámicamente el número de episodios o capítulos consumidos desde la interfaz principal.
3. **Búsqueda y Filtrado:** El sistema permitirá realizar consultas SQL a la base de datos para buscar obras concretas o aplicar filtros.

## Requisitos No Funcionales

1. **Persistencia:** Todos los datos deben almacenarse en una base de datos MySQL. Se requiere uso intensivo de sentencias preparadas para evitar inyección SQL.
2. **Interfaz de Usuario:** La interfaz debe ser desarrollada con JavaFX, utilizando contenedores como VBox, HBox y GridPane para una correcta alineación visual.
3. **Control de Versiones:** El proyecto se gestionará a través de Git y se alojará en un repositorio remoto.
