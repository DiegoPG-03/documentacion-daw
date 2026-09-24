---
sidebar_position: 1
---

# Diseño y Diagrama de Clases

La aplicación sigue un estricto patrón MVC. A continuación, se detallan las clases principales del modelo utilizando sintaxis de Mermaid (soportada de forma nativa por muchos generadores estáticos).

## Entidades Principales (Modelo)

* `Obra (Abstract)`: Clase base abstracta que contiene atributos comunes como `id`, `titulo`, `genero`, y `estado`.
* `Anime (extends Obra)`: Añade atributos específicos como `episodiosVistos` y `estudioAnimacion`.
* `Manga (extends Obra)`: Añade atributos como `capitulosLeidos` y `mangaka`.
* `Coleccion`: Representa la lista local (gestionada mediante un `ArrayList` o `HashMap` en memoria) antes de volcarse a la base de datos.

```mermaid
classDiagram
  Obra <|-- Anime
  Obra <|-- Manga
  Usuario "1" *-- "many" Obra : Coleccion

  class Obra{
    +String titulo
    +String estado
  }
  class Anime{
    +int episodiosVistos
    +String estudioAnimacion
  }
  class Manga{
    +int capitulosLeidos
    +String mangaka
  }
