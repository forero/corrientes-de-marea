# Corrientes de marea

Simulador interactivo de cómo un satélite (una galaxia enana o un cúmulo
globular) pierde estrellas por efecto de marea al orbitar el halo de la Vía
Láctea, formando una corriente delantera y trasera. Construido para el
Taller 13 Parte B de Introducción a la Astronomía General (Universidad de
los Andes, 202620).

Página en vivo: https://forero.github.io/corrientes-de-marea/

## Qué muestra

- **Vista de frente** (desde arriba) y **vista de canto** (de lado) de la
  órbita del satélite y la corriente, con el disco galáctico marcado de
  forma esquemática en ambas para ubicar la perspectiva.
- Los contornos de igual potencial del halo, achatados por el parámetro
  `q`, dibujados directamente en la vista de canto.
- Una vista del cielo simulada (longitud y latitud vistas desde el Sol, a
  8 kpc del centro), donde se nota si la corriente precesa o no según la
  forma del halo.
- Controles de masa del satélite, radio de apogaláctico, excentricidad
  orbital, achatamiento del halo y inclinación de la órbita.

## Modelo físico

Halo de materia oscura con curva de rotación plana (`v_max = 220 km/s`,
el mismo valor usado en el Taller 13A para pesar la Galaxia), descrito por
un potencial logarítmico achatado por `q`. El satélite y las estrellas
liberadas en el radio de marea (fórmula de Jacobi) se integran como
partículas de prueba en ese potencial con un integrador leapfrog. Es un
modelo de juguete para fines de enseñanza, no una simulación de
investigación.

Todo el código es una sola página HTML autocontenida (`index.html`), sin
dependencias externas.
