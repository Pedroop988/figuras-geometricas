# Figuras Geométricas

Este repositorio contiene un script en Python para calcular el área de diversas figuras geométricas utilizando el enfoque de programación orientada a objetos.

## Desarrollador

| Apellidos y nombres             |
| ------------------------------- |
| Ortega Poma Pedro Claudio       |

## Propósito del repositorio

El propósito de este repositorio es implementar un sistema para calcular el área de diferentes figuras geométricas, como rectángulos, triángulos y círculos, mediante clases en Python.

## Cambios realizados

- Se corrigió el nombre del módulo para seguir la convención de estilo snake_case.
- Se ajustó el espaciado en las definiciones de las clases y funciones.
- Se agregó documentación a las clases y métodos siguiendo las normas de PEP8.
- Se removió la instrucción `pass` innecesaria en el método `calcular_area` de la clase `FiguraGeometrica`.
- Se mejoró la legibilidad del código con comentarios explicativos.

## Estructura del código

El código está dividido en las siguientes clases:

1. **FiguraGeometrica**: Clase abstracta que define el método `calcular_area`, que debe ser implementado por las clases hijas.
2. **Rectangulo**: Clase hija de `FiguraGeometrica` que implementa el cálculo del área de un rectángulo.
3. **Triangulo**: Clase hija de `FiguraGeometrica` que implementa el cálculo del área de un triángulo.
4. **Circulo**: Clase hija de `FiguraGeometrica` que implementa el cálculo del área de un círculo.

## Ejemplo de uso

```python
# Variables globales
BASE_RECTANGULO = 10
ALTURA_RECTANGULO = 5
BASE_TRIANGULO = 7
ALTURA_TRIANGULO = 4
RADIO_CIRCULO = 3

# Ejecución principal
if __name__ == "__main__":
    rectangulo = Rectangulo(BASE_RECTANGULO, ALTURA_RECTANGULO)
    triangulo = Triangulo(BASE_TRIANGULO, ALTURA_TRIANGULO)
    circulo = Circulo(RADIO_CIRCULO)

    print(f"El área del rectángulo es: {rectangulo.calcular_area()}")
    print(f"El área del triángulo es: {triangulo.calcular_area()}")
    print(f"El área del círculo es: {circulo.calcular_area()}")
