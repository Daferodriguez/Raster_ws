# Taller raster

## Propósito

Comprender algunos aspectos fundamentales del paradigma de rasterización.

## Tareas

Emplee coordenadas baricéntricas para:

1. Rasterizar un triángulo; y,
2. Sombrear su superficie a partir de los colores de sus vértices.

Referencias:

* [The barycentric conspiracy](https://fgiesen.wordpress.com/2013/02/06/the-barycentric-conspirac/)
* [Rasterization stage](https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/rasterization-stage)

Opcionales:

1. Implementar un [algoritmo de anti-aliasing](https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/rasterization-practical-implementation) para sus aristas; y,
2. Sombrear su superficie mediante su [mapa de profundidad](https://en.wikipedia.org/wiki/Depth_map).

Implemente la función ```triangleRaster()``` del sketch adjunto para tal efecto, requiere la librería [frames](https://github.com/VisualComputing/frames/releases).

## Integrantes

Dos, o máximo tres si van a realizar al menos un opcional.

Complete la tabla:

| Integrante | github nick |
|------------|-------------|
|      Sergio Alexander Gil Medina    |      sagilm       |
|      John Alexander Hernandez Carrero      |      joahernandezca       |
|      David Felipe Rodriguez Rodriguez      |      daferodriguez       |

## Discusión
Se usaron algoritmos de orientacion para determinar el color que representa cada uno de los vertices del triángulo, y la distancia desde los vertices para determinar el color de cada uno de los pixeles que conforman el interior del triángulo.

El antialiasing se realiza determinando de forma más precisa el rango de color que se usa, coloreando con un rango menor aquellos pixeles que se encuentran más proximos a las aristas del triángulo.

El antialiasing puede visualizarse mejor si se presiona la tecla 'a' en la ejecución.

Con anti Aliasing:

![alt text](https://github.com/Daferodriguez/Raster_ws/blob/master/AntiAliasing.JPG)

## Referencias
- https://fgiesen.wordpress.com/2013/02/08/triangle-rasterization-in-practice/
- http://www.dma.fi.upm.es/personal/mabellanas/tfcs/kirkpatrick/Aplicacion/algoritmos.htm#kirkpatrick
- https://www.youtube.com/watch?v=GvLEAHRmPl0
- https://www.youtube.com/watch?v=C_yh7gw7tbg

## Entrega

* Modo de entrega: [Fork](https://help.github.com/articles/fork-a-repo/) la plantilla en las cuentas de los integrantes.
* Plazo: 30/9/18 a las 24h.
