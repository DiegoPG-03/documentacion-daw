---
sidebar_position: 1
---

# Análisis de Caja Blanca

Durante el desarrollo, se han aplicado técnicas de caja blanca para garantizar que todos los caminos lógicos del código sean cubiertos en las pruebas unitarias.

## Ejemplo de Análisis: Método `actualizarProgreso`

Analicemos la lógica del siguiente método en Java:

```java
public void actualizarProgreso(int nuevosCapitulos) {
    if (nuevosCapitulos < 0) {
        throw new IllegalArgumentException("No se pueden sumar valores negativos");
    }
    if (this.capitulosVistos + nuevosCapitulos >= this.totalCapitulos) {
        this.capitulosVistos = this.totalCapitulos;
        this.estado = "Completado";
    } else {
        this.capitulosVistos += nuevosCapitulos;
    }
}
