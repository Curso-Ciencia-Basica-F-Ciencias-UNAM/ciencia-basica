---
title: "Práctica 1"
date: 2023-07-24T18:06:09-06:00
weight: 11
---

# Práctica 1

**Movimiento en 1 dimensión, movimiento parabólico y juego de cañón**

<!-- {{<hint info>}}  -->
<!-- **Contenido:** 11 videos   -->
<!-- **Duración estimada:** 1 hora 24 minutos -->
<!-- {{</hint>}} -->

---

## Introducción 

Esta práctica consiste de dos partes. En la primera parte vamos a construir en NetLogo un modelo de movimiento en 1 dimensión. Y en la segunda parte vamos a construir un modelo de movimiento en 2 dimensiones (movimiento parabólico) y extenderlo a un juego de tiro de un cañon.

---

## Parte I: Movimiento en 1D {#mov-1D}

{{<hint info>}}
**Contenido:** 4 videos  
**Duración estimada:** 27 minutos
{{</hint>}}

![Gif modelo de movimiento en 1 dimension](/img/1D.gif)

#### Repaso y definición del modelo

{{<youtube id="wBd_9hC8Pjg">}}

#### Procedimiento `setup`

{{<youtube id="YxNLfj0ju9o">}}

#### Procedimiento `go`

{{<youtube id="V72aePovv7U">}}

#### Gráficas

{{<youtube id="KTkH_tgjdB4">}}

{{<hint danger>}}**Corrección**  
En el minuto 2:42 cuando se agrega la gráfica de velocidad vs tiempo las etiquetas del eje de las X y del eje de las Y se pusieron invertidas. En _X axis label_ debe ir `tiempo` y en _Y axis label_ debe ir `velocidad`. 
{{</hint>}}

{{<hint warning>}}**Explora el modelo**  
Modifica los parámetros del modelo y observa qué pasa con las gráficas. ¿Cómo cambian las gráficas cuando mueves el parámetro `aceleracion` mientras el modelo está corriendo?
{{</hint>}}

---

## Parte II: Movimiento en 2D {#mov-2D}

{{<hint info>}}
**Contenido:** 7 videos  
**Duración estimada:** 57 minutos
{{</hint>}}

### Movimiento parabólico

![Gif modelo de movimiento parabólico](/img/parabolico.gif)

#### Repaso y definición del modelo

{{<youtube id="RWHukr7PNwA">}}

#### Extensión a movimiento parabólico (parte 1)

{{<youtube id="CT3E7m8GUC4">}}

{{<hint danger>}}**Corrección**  
En el minuto 8:24 se menciona que el valor de _min-pycor_ es 1, sin embargo, el valor correcto que se usa es -1.
{{</hint>}}

#### Extensión a movimiento parabólico (parte 2)

{{<youtube id="mHPH2vTdqjg">}}

#### Gráficas

{{<youtube id="SGo8Ln_AdFQ">}}

{{<hint warning>}}**Explora el modelo**  
Modifica los parámetros del modelo y observa qué pasa con las gráficas.
- ¿Qué pasa si aumentas la aceleración de la gravedad? Pon el valor de `aceleracion-x` igual a 0 y modifica el valor de `aceleracion-y`.
- ¿Qué pasa si modificas el valor de `aceleracion-x`? ¿Qué podría representar que la aceleración en x fuera distinta de cero?
{{</hint>}}

### Juego de cañon

![Gif modelo de juego de cañón](/img/cañón.gif)

#### Presentación del juego

{{<youtube id="o4Ss3189MHw">}}

#### Extensión a juego de cañón (parte 1)

{{<youtube id="x-27lAT1cmc">}}

#### Extensión a juego de cañón (parte 2)

{{<youtube id="9TeAzqqtgH0">}}

{{<hint warning>}}**Modifica el modelo**  
Puedes intentar modificar el juego de multiples formas:
- cambia la forma (`shape`) del cañon o del objetivo
- crea un objetivo que sólo se pueda estar en el suelo (que su `ycor` sea cero)
- cambia el "paisaje" cambiando el color de los parches (`pcolor`) de fondo
- haz que el objetivo se mueva
{{</hint>}}
