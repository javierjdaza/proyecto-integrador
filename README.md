# 🔬 Proyecto de Clustering de Proyectos – Concentrix

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.2-orange?logo=scikit-learn)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-2.2.1-blue?logo=pandas)](https://pandas.pydata.org/)
[![UMAP](https://img.shields.io/badge/UMAP-0.5.4-purple?logo=python)](https://umap-learn.readthedocs.io/)
[![PCA](https://img.shields.io/badge/PCA-built--in-lightgrey?logo=python)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/status-active-success)]()

---

## 📊 Análisis de Clustering de Proyectos – Concentrix

Este proyecto aplica técnicas de reducción dimensional (UMAP y PCA) combinadas con **K-Means Clustering** para segmentar los proyectos de Concentrix según variables clave como:

- `project_priority`
- `avg_risk_exposure`
- `total_headcount`
- `num_tasks`
- `duration`

### 🔍 Metodología

- **Reducción dimensional**:
  - **UMAP**: preserva la estructura local, útil para identificar patrones complejos o no lineales.
  - **PCA**: captura la varianza global, útil para visualizaciones lineales y explicabilidad.
- **Clustering**:
  - Se aplicó **K-Means** en el espacio reducido para detectar patrones naturales en los proyectos.

### 📌 Resultados principales

| Enfoque | Cluster 0 | Cluster 1 |
|--------|-----------|-----------|
| **UMAP** | Proyectos complejos, con alta prioridad, riesgo elevado, duración extensa y mayor número de tareas. | Proyectos rutinarios, con riesgo muy bajo, menor duración y carga operativa. |
| **PCA** | Proyectos grandes, con headcount alto, duración prolongada y exposición a riesgo elevada. | Proyectos operativos, simples, con baja exposición al riesgo y menor complejidad. |

> Ambos enfoques coinciden en distinguir dos perfiles bien diferenciados:
> - **Cluster 0**: Proyectos estratégicos, complejos y de alto impacto.
> - **Cluster 1**: Proyectos estándar, operativos y de bajo riesgo.

### 📁 Archivos relevantes

- [`kmeans_cluster_analysis_UMAP.md`](./kmeans_cluster_analysis_UMAP.md) – Análisis detallado con UMAP
- [`kmeans_cluster_analysis_PCA.md`](./kmeans_cluster_analysis_PCA.md) – Análisis detallado con PCA

---

## 👥 Autores

- **Javier Daza**  
- **María Sofía Uribe**  
- **Pablo Andrés Jimeno**  

