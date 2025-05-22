# Análisis (Kmeans + UMAP)

---

## Cluster 0 – “Proyectos complejos, de alta prioridad y riesgo”

**Tamaño del cluster:** 730 proyectos

| Variable             | Promedio | Comentario                                                                                                                                                                       |
| -------------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Prioridad**        | 2.91     | Moderadamente alta. El percentil 50 (mediana) es 3, indicando que la mayoría de los proyectos están clasificados como prioritarios. Hay presencia de prioridad máxima (4).       |
| **Riesgo**           | 4.17     | Riesgo medio-alto. Percentiles 25%-75% oscilan entre 2.17 y 5.82. Algunos casos llegan hasta 9.5, indicando exposición significativa.                                            |
| **Headcount**        | 87.31    | Requiere una cantidad considerable de recursos. El rango intercuartílico es estrecho (51, 51, 51), pero con una máxima muy alta (1593), indicando outliers en grandes proyectos. |
| **Número de tareas** | 85.35    | Alta carga operativa. La media y la mediana son significativamente mayores respecto al cluster 1.                                                                                |
| **Duración (días)**  | 122.39   | Proyectos más largos en el tiempo. Media alta, aunque con variabilidad considerable (0 a 587 días).                                                                              |

---

## Cluster 1 – “Proyectos estándares, de bajo riesgo”

**Tamaño del cluster:** 751 proyectos

| Variable             | Promedio | Comentario                                                                                                                                                                                        |
| -------------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Prioridad**        | 2.99     | Muy concentrado en 3. Bajo desvío estándar (0.036), lo que indica poca variabilidad: estos proyectos tienen casi todos prioridad media.                                                           |
| **Riesgo**           | 0.27     | Extremadamente bajo. La mayoría tiene riesgo cercano a 0.                                                                                                                                         |
| **Headcount**        | 151.15   | Media alta, pero con altísima dispersión (std = 738). Esto sugiere outliers con equipos enormes (hasta 15,000 personas), lo que podría deberse a errores o a proyectos operativos de gran escala. |
| **Número de tareas** | 42.56    | Aproximadamente la mitad del cluster 0. Menor carga operativa.                                                                                                                                    |
| **Duración (días)**  | 72.68    | Proyectos de duración media-corta. El percentil 75 es 98.5 días, significativamente menor que el del cluster 0.                                                                                   |

---
