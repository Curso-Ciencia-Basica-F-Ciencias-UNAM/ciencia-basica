---
title: "Práctica 6"
date: 2023-10-18T00:11:05-06:00
weight: 16
---

# Práctica 6

**Teoría cinética de los gases**

{{<hint info>}}
**Contenido:** 9 videos  
**Duración estimada:** 1 hora 33 minutos 
{{</hint>}}

---

## Introducción

Esta práctica consiste de dos partes. En la primera parte vamos a construir un modelo de gas ideal sin interacciones entre partículas y exploraremos como se relacionan las variables macroscópicas de los gases: presión, temperatura y volumen. En la segunda parte vamos a extender nuestro modelo para considerar qué ocurre cuando ocurren interacciones entre partículas, particularmente choques elásticos.

![Modelo cinética de los gases](/img/cinetica-gases.gif)

## Parte I

### Repaso y definición del modelo

{{<youtube id="7eF-dTDioSg">}}

### Procedimiento `setup`

{{<youtube id="OUyiEwX1R7w">}}

### Procedimiento `go`

{{<youtube id="NtiRfKE-IWs">}}

### Propiedades macroscópicas

{{<youtube id="xfibS7JCSoQ">}}

### Experimento presión-volumen

{{<youtube id="qFMhpRWAYE0">}}

### Graficar en python

En esta sección usamos algunos paquetes de python para hacer nuestra gráfica de presión contra volumen. Sientanse en la libertad de hacer sus gráficas en cualquier otro lenguaje/programa que ustedes quieran (e.g., R, julia, Excel, etc). Si no tienen python instalado y/o no quieren/pueden instalar los paquetes que se usan pueden correrlo desde un notebook de [Google Colbaoratory](https://colab.research.google.com/).

{{<hint warning>}}**Installación de pandas y matplotlib**  

Si están usando python desde su computadora deben instalar los paquetes `pandas` y `matplotlib`:

```
pip install pandas matplotlib
```
{{</hint>}}

{{<youtube id="k-dqCK9dSuo">}}

{{<hint info>}}**Descarga**  
[Descarga el script de python para generar la gráfica de presión-volumen](/descargas/presion-volumen.py). 

Si te abre el archivo en un tu navegador da click derecho y luego selecciona "Guardar página como...".

{{</hint>}}


<!-- ### Experimento presión-temperatura y gráfica en python -->

<!-- {{<youtube id="OjFquOndU88">}} -->

## Parte II

### Explicación extensión del modelo

{{<youtube id="rhsZpp63Ot4">}}

{{<hint info>}}**Para saber más**  
Si quieres saber más sobre las colisiones elásticas y de donde viene la expresión que utilizamos para modelarla puedes consultar la [página de wikipedia sobre colisiones elásticas](https://en.wikipedia.org/wiki/Elastic_collision#Two-dimensional_collision_with_two_moving_objects).
{{</hint>}}

### Colisiones entre partículas

{{<youtube id="2RgjIsOIOcI">}}

### Detalles para facilitar la exploración

{{<youtube id="rntmpSYri2w">}}
