# Análisis de Clusters (KMeans + PCA)

Este documento resume el análisis detallado de los dos clusters obtenidos tras aplicar K-Means sobre los componentes principales (PCA) del dataset de proyectos de Concentrix.

---

## 🔵 Cluster 0 – “Proyectos grandes, de alto riesgo y duración extensa”

**Tamaño del cluster:** 445 proyectos

| Variable             | Promedio | Comentario                                                                                                                                                   |
| -------------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Prioridad**        | 2.83     | Predominan proyectos de prioridad media (valor 3). Hay algunos de prioridad mínima (1), pero también casos de prioridad alta (4).                            |
| **Riesgo**           | 4.54     | Riesgo medio-alto a alto. El rango intercuartílico va de 2.35 a 6.65, con valores máximos de hasta 9.5.                                                      |
| **Headcount**        | 215.05   | Significativamente alto. El valor máximo (15,000) indica la presencia de mega proyectos o outliers.                                                          |
| **Número de tareas** | 112.05   | Muy alta carga operativa. La media y mediana muestran proyectos con muchas tareas involucradas.                                                              |
| **Duración (días)**  | 154.30   | Proyectos extensos. El percentil 75 es 194 días, y la media es la más alta entre ambos clusters. Claramente representan proyectos más complejos y duraderos. |

---

## 🟠 Cluster 1 – “Proyectos operativos, de bajo riesgo y duración corta”

**Tamaño del cluster:** 1036 proyectos

| Variable             | Promedio | Comentario                                                                                                      |
| -------------------- | -------- | --------------------------------------------------------------------------------------------------------------- |
| **Prioridad**        | 3.01     | Muy concentrado en prioridad 3. Baja desviación estándar (0.14),                                                |
| **Riesgo**           | 1.19     | Bajo riesgo. La mayoría de los proyectos tienen exposición al riesgo entre 0 y 1.75.                            |
| **Headcount**        | 78.72    | Menor en promedio. Aunque hay outliers (hasta 2,196), la mayoría requiere menos personal que los del cluster 0. |
| **Número de tareas** | 42.86    | Carga operativa baja.                                                                                           |
| **Duración (días)**  | 72.65    | Proyectos de duración media a corta. Percentiles intercuartílicos entre 43 y 96 días.                           |

---

## ✅ Conclusión comparativa PCA

-   El cluster 0 agrupa proyectos **más exigentes en recursos, duración y riesgo**, probablemente estratégicos o personalizados.
-   El cluster 1 representa proyectos **más estandarizados y operativos**, con bajo riesgo y duración corta.

Este resultado es coherente con el análisis UMAP, pero el enfoque PCA tiende a separar con más fuerza los proyectos extremos en duración y headcount, como muestra la diferencia de medias más pronunciada.
