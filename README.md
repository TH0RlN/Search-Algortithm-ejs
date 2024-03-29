# Ejercicios de algoritmos de busqueda

### Búsqueda bidireccional

![1710169898368](image/README/1710169898368.png)

|   | Desde Ourense (OU)                                                                                                                                         | Desde Calatayud (CL)                                                                                                                                          |
| - | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | **Frontera:** PO.175, BE.236<br />**Explorados:** OU.0                                                                                        | **Frontera:** SO.91, OS.140<br /> **Explorados:** CL.0                                                                                          |
| 2 | **F:** *BE.236*, LE.288, *~~BE.350~~*<br />**E:** OU.0, PO.175                                                                          | **F:** *OS.140*, *~~OS.149~~*, LG.197, BG.234<br />**E:** CL.0, SO.91                                                                        |
| 3 | **F:** *LE.288*, *~~LE.311~~*, PA.348, VA.348<br />**E:** OU.0, PO.175, BE.236                                                            | **F:** LG.197, BG.234, AR.198<br />**E:** CL.0, SO.91, OS.140                                                                                     |
| 4 | **F:** PA.348, VA.348, OR.409, *~~PA.415~~*<br />**E:** OU.0, PO.175, BE.236, LE.288                                                       | **F:** *BG.234*, AR.198, *~~BG.347~~*<br />**E:** CL.0, SO.91, OS.140, LG.197                                                                |
| 5 | **F:** *VA.348*, *~~OR.409~~*, *~~LE.419~~*, *OR.397*, BG.440, *~~VA.396~~*<br />**E:** OU.0, PO.175, BE.236, *LE.288*, PA.348 | **F:** *AR.198*, *~~AR.288~~*, PA.326, OR.293<br />**E:** CL.0, SO.91, OS.140, LG.197, BG.234                                                |
| 6 | **F:** *OR.397*, ~~*BE.440*~~, *~~PA.396~~*, AR.443<br />**E:** OU.0, PO.175, *BE.236*, LE.288, *PA.348*, VA.348                  | **F:** PA.326, OR.293, VA.293, *~~BG.282~~*<br />**E:** CL.0, SO.91, OS.140, LG.197, *BG.234*, AR.198                                        |
| 7 | **F:** AR.443, BG.456, *~~PA.466~~*<br />**E:** OU.0, PO.175, BE.236, LE.288, *PA.348*, VA.348, OR.397                                    | **F:** *OR.293, VA.293, ~~OR.375~~*, LE.457, BE.348, *~~VA.374~~*<br />**E:** CL.0, SO.91, OS.140, LG.197, BG.234, **AR.198**, PA.326 |
| 8 | **F:** BG.456, BG, OS<br />**E:** OU.0, PO.175, BE.236, LE.288, PA.348, VA.348, OR.397, **AR.443**                                      |                                                                                                                                                               |

**Solución:** OU → BE → VA → AR → OS → CL

<img src='image/README/1710179095465.png' style='height:600px'>
<img src='image/README/1710179175048.png' style='width:600px'>

### Búsqueda A*

Dado o seguinte mapa, busca a solución mediante o algoritmo de búsqueda A*

* **E:** Entrada
* **S:** Salida
* **#:** Muro

| S      | &nbsp;      | &nbsp;      | &nbsp;      | &nbsp; |
| ------ | ----------- | ----------- | ----------- | ------ |
|        | **#** | **#** | **#** |        |
|        | **#** | **E** | **#** |        |
|        | **#** |             |             |        |
| &nbsp; |             |             |             |        |

* **g**: coste entrada → nodo
* **h**: distanca nodo → salida
* **f**: g + h
* **k**: coste movimiento
* **n**: orden exploración

<img src='image/README/1710235987731.png' style='height:300px'>



<img src='image/README/1710235222306.png' style='height:600px'>
