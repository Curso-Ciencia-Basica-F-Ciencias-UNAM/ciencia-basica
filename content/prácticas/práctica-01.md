---
title: "Práctica 1"
date: 2023-07-24T18:06:09-06:00
weight: 11
---

# Practica 1

**Movimiento en 1 dimensión, movimiento parabólico y juego de cañón**

{{<hint info>}} 
**Contenido:** 11 videos  
**Duración estimada:** 1 hora 24 minutos
{{</hint>}}

---

## Introducción

En esta práctica vamos a construir y explorar tres modelos en NetLogo: 

1. modelo del movimiento en 1 dimensión, 
2. modelo del movimiento parabólico y 
3. juego de lanzamiento de un cañon.

## Movimiento en 1 dimensión {#mov-1D}

### Repaso y definición del modelo

{{<youtube id="wBd_9hC8Pjg">}}

### Procedimiento `setup`

{{<youtube id="YxNLfj0ju9o">}}

### Procedimiento `go`

{{<youtube id="V72aePovv7U">}}

### Gráficas

{{<youtube id="KTkH_tgjdB4">}}

{{<hint warning>}}**Explora el modelo**  
Modifica los parámetros del modelo y observa qué pasa con las gráficas. ¿Cómo cambian las gráficas cuando mueves el parámetro `aceleracion` mientras el modelo está corriendo?
{{</hint>}}

## Movimiento parabólico

### Repaso y definición del modelo

{{<youtube id="RWHukr7PNwA">}}

### Extensión a movimiento parabólico (parte 1)

{{<youtube id="CT3E7m8GUC4">}}

### Extensión a movimiento parabólico (parte 2)

{{<youtube id="mHPH2vTdqjg">}}

### Gráficas

{{<youtube id="SGo8Ln_AdFQ">}}

{{<hint warning>}}**Explora el modelo**  
Modifica los parámetros del modelo y observa qué pasa con las gráficas.
- ¿Qué pasa si aumentas la aceleración de la gravedad? Pon el valor de `aceleracion-x` igual a 0 y modifica el valor de `aceleracion-y`.
- ¿Qué pasa si modificas el valor de `aceleracion-x`? ¿Qué podría representar que la aceleración en x fuera distinta de cero?
{{</hint>}}


## Juego de cañón

### Presentación del juego

{{<youtube id="o4Ss3189MHw">}}

### Extensión a juego de cañón (parte 1)

{{<youtube id="x-27lAT1cmc">}}

### Extensión a juego de cañón (parte 2)

{{<youtube id="9TeAzqqtgH0">}}

{{<hint warning>}}**Modifica el modelo**  
Puedes intentar modificar el juego de multiples formas:
- cambia la forma (`shape`) del cañon o del objetivo
- crea un objetivo que sólo se pueda estar en el suelo (que su `ycor` sea cero)
- cambia el "paisaje" cambiando el color de los parches (`pcolor`) de fondo
- haz que el objetivo se mueva
{{</hint>}}
