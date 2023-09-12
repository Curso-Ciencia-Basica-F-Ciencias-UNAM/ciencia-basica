---
title: "Práctica 3"
date: 2023-09-11T21:10:52-06:00
weight: 13
---

# Práctica 3

**Ley de gravitación universal**

{{<hint info>}}
**Contenido:** 12 videos  
**Duración estimada:** 1 hora 51 minutos 
{{</hint>}}

---

## Introducción

En esta práctica vamos a construir un modelo para explorar a cuerpos interactuando bajo la Ley de gravitación universal. Primero construiremos un modelo para explorar la interacción de 2 cuerpos y luego lo extenderemos a 3 cuerpos, lo cual nos permitirá también explorar la idea de dinámicas caóticas.

![sistema de 2 orbitas iguales](/img/2-orbitas-iguales.gif)
![sistema sol-tierra-luna](/img/sol-tierra-luna.gif)
![solución periódica 3 cuerpos BA2](/img/BA2.gif)
![dinámica caótica](/img/euler-caos.gif)

## Repaso y definición del modelo

{{<youtube id="47JdDyF9J-k">}}

## Explicación del modelo

{{<youtube id="OkXN5Bj-FWo">}}

## Procedimiento setup

{{<youtube id="564pocmXQH8">}}

## Procedimiento go

{{<youtube id="aXj0EErbzfE">}}

## Trazo de órbitas y recentrar

{{<youtube id="AhRPwxBkqig">}}

## Difuminar trazo

{{<youtube id="M7vcvlwUSU4">}}

## Guardar condiciones iniciales

{{<youtube id="TxXyKOV3j5Q">}}

{{< tabs "guardar-condiciones-iniciales" >}}
{{< tab "2 orbitas iguales" >}}
```
;;;; cuerpo 1
set cuerpo1? True
set m1 200
set x1 -40
set y1 0
set vx1 0
set vy1 0
set s1 10

;;;; cuerpo 2
set cuerpo2? True
set m2 200
set x2 40
set y2 0
set vx2 0
set vy2 2
set s2 10

;;;; cuerpo 3
set cuerpo3? False

```
{{< /tab >}}
{{< tab "sol-tierra" >}}
```
set k 1

;;;; cuerpo 1
set cuerpo1? True
set m1 200
set x1 0
set y1 0
set vx1 0
set vy1 0
set s1 20

;;;; cuerpo 2
set cuerpo2? True
set m2 1
set x2 60
set y2 0
set vx2 0
set vy2 2
set s2 5

;;;;; cuerpo 3
set cuerpo3? False
```
{{< /tab >}}
{{< /tabs >}}

## Extensión a 3 cuerpos

{{<youtube id="BlLCGsCq_kk">}}

{{< tabs "extension-a-3-cuerpos" >}}
{{< tab "sol-tierra-luna" >}}
```
;;; cuerpo 1
set cuerpo1? True 
set m1 199 
set vx1 0 
set vy1 0 
set x1 0  
set y1 0
set s1 20 

;;; cuerpo 2
set cuerpo2? True 
set m2 1
set vx2 0 
set vy2 1.6 
set x2 60  
set y2 0
set s2 5

;;; cuerpo 3
set cuerpo3? True
set m3 0.5
set vx3 0 
set vy3 2 
set x3 65  
set y3 0
set s3 2
```
{{< /tab >}}
{{< /tabs >}}

## Soluciones periódicas problema de los 3 cuerpos (parte 1)

{{<youtube id="0Pa-jCD8P7k">}}

{{<hint warning>}}**Galería de soluciones periódicas del problema de los 3 cuerpos**

Página con distintas soluciones periódicas del problema de los 3 cuerpos que se usa en el video: [3-BODY GALLERY](http://three-body.ipb.ac.rs/)
{{</hint>}}

{{< tabs "soluciones-periodicas-3-cuerpos" >}}
{{< tab "figura 8" >}}
```
set k 40

;;; cuerpo 1
set cuerpo1? True
set m1 1
set x1 -1
set y1 0
set vx1 0.347111
set vy1 0.532728
set s1 5

;;; cuerpo 2
set cuerpo2? True
set m2 1
set x2 1
set y2 0
set vx2 0.347111
set vy2 0.532728
set s2 5

;;; cuerpo 3
set cuerpo3? True
set m3 1
set x3 0
set y3 0
set vx3 -0.694222
set vy3 -1.065456
set s3 5
```
{{< /tab >}}
{{< tab "2 orbitas iguales (actualizado)" >}}
```
set k 1

;;;; cuerpo 1
set cuerpo1? True
set m1 200
set x1 -40
set y1 0
set vx1 0
set vy1 0
set s1 10

;;;; cuerpo 2
set cuerpo2? True
set m2 200
set x2 40
set y2 0
set vx2 0
set vy2 2
set s2 10

;;;; cuerpo 3
set cuerpo3? False
```
{{< /tab >}}
{{< tab "sol-tierra (actualizado)" >}}
```
set k 1

;;;; cuerpo 1
set cuerpo1? True
set m1 200
set x1 0
set y1 0
set vx1 0
set vy1 0
set s1 20

;;;; cuerpo 2
set cuerpo2? True
set m2 1
set x2 60
set y2 0
set vx2 0
set vy2 2
set s2 5

;;;;; cuerpo 3
set cuerpo3? False
```
{{< /tab >}}
{{< tab "sol-tierra-luna (actualizado)" >}}
```
set k 1

;;; cuerpo 1
set cuerpo1? True 
set m1 199 
set vx1 0 
set vy1 0 
set x1 0  
set y1 0
set s1 20 
;;; cuerpo 2
set cuerpo2? True 
set m2 1
set vx2 0 
set vy2 1.6 
set x2 60  
set y2 0
set s2 5
;;; cuerpo 3
set cuerpo3? True
set m3 0.5
set vx3 0 
set vy3 2 
set x3 65  
set y3 0
set s3 2
```
{{< /tab >}}
{{< /tabs >}}

## Soluciones periódicas problema de los 3 cuerpos (parte 2)

{{<youtube id="8e-NmzqAkoM">}}

{{< tabs "soluciones-periodicas-3-cuerpos-2" >}}
{{< tab "BA2" >}}
```
set k 40

;;; cuerpo 1
set cuerpo1? True
set m1 1
set x1 0.3361300950
set y1 0
set vx1 0
set vy1 1.5324315370
set s1 5

;;; cuerpo 2
set cuerpo2? True
set m2 1
set x2 0.7699893804
set y2 0
set vx2 0
set vy2 -0.6287350978
set s2 5

;;; cuerpo 3
set cuerpo3? True
set m3 1
set x3 -1.1061194753
set y3 0
set vx3 0
set vy3 -0.9036964391
set s3 5
```
{{< /tab >}}
{{< /tabs >}}

## Dinámicas caóticas

{{<youtube id="nakRtavmYn8">}}
{{< tabs "dinamicas-caoticas" >}}
{{< tab "euler" >}}
```
;;; parametros generales
set delta-t 0.01
set k 50

;;; cuerpo 1
set cuerpo1? True 
set m1 1 
set vx1 0
set vy1 ( - 1 )
set x1 -1
set y1 0
set s1 5
;;; cuerpo 2
set cuerpo2? True 
set m2 1
set vx2 0 
set vy2 0
set x2 0
set y2 0
set s2 5
;;; cuerpo 3
set cuerpo3? True
set m3 1
set vx3 0 
set vy3 1
set x3 1
set y3 0
set s3 5
```
{{< /tab >}}
{{< tab "larange" >}}
```
;;; parametros generales
set delta-t 0.001
set k 30
let v 0.5

;;; cuerpo 1
set cuerpo1? True 
set m1 1 
set vx1 v
set vy1 0
set x1 0
set y1 1
set s1 5
;;; cuerpo 2
set cuerpo2? True 
set m2 1
set vx2 ( - v * sin 30 )
set vy2 ( - v * cos 30 )
set x2  ( ( sqrt 3 ) / 2 )
set y2  (- 1 / 2)
set s2 5
;;; cuerpo 3
set cuerpo3? True
set m3 1
set vx3 (- v * sin 30)
set vy3 (  v * cos 30)
set x3  (- ( sqrt 3 ) / 2)
set y3  (- 1 / 2)
set s3 5
```
{{< /tab >}}
{{< /tabs >}}



{{<hint warning>}}**Material complementario**  
Si les interesa saber más sobre el problema de los 3 cuerpos y las dinámicas caóticas pueden consultar los siguientes videos:
- [Newton’s three-body problem explained - Fabio Pacucci](https://www.youtube.com/watch?v=D89ngRr4uZg)
- [Chaos and the Three Body Problem](https://www.youtube.com/watch?v=mm3I4m8YsnM)
{{</hint>}}

## Actividad de evidencia

{{<youtube id="BlLCGsCq_kk">}}

{{<hint warning>}}**Galería de soluciones periódicas del problema de los 3 cuerpos**

Página con distintas soluciones periódicas del problema de los 3 cuerpos que se usa en el video: [3-BODY GALLERY](http://three-body.ipb.ac.rs/)
{{</hint>}}

{{< tabs "actividad-evidencia" >}}
{{< tab "Esqueleto de botón de condiciones iniciales" >}}
```
;;; parametros generales
set delta-t          ;; <- poner valor
set k                ;; <- poner valor

;;; cuerpo 1
set cuerpo1? True
set m1 1
set vx1              ;; <- poner valor
set vy1              ;; <- poner valor
set x1               ;; <- poner valor
set y1               ;; <- poner valor
set s1 5
;;; cuerpo 2
set cuerpo2? True 
set m2 1
set vx2              ;; <- poner valor
set vy2              ;; <- poner valor
set x2               ;; <- poner valor
set y2               ;; <- poner valor
set s2 5
;;; cuerpo 3
set cuerpo3? True
set m3 1
set vx3              ;; <- poner valor
set vy3              ;; <- poner valor
set x3               ;; <- poner valor
set y3               ;; <- poner valor
set s3 5
```
{{< /tab >}}
{{< /tabs >}}
