# Análisis del Clustering en el Dataset Iris

- **Contexto de procesamiento:** El análisis se realizó utilizando una sesión de PySpark en un cluster HPC, empleando la cuota personal del usuario para garantizar un procesamiento eficiente y la correcta gestión de recursos.

Se evaluó el **dataset Iris** usando el método del codo y visualizaciones de clusters para distintos valores de k.

- **Método del codo (WSSSE):** La gráfica sugiere que matemáticamente k podría ser mayor (≈6), pero la reducción de error más allá de k=3–4 es mínima.  

- **Visualización de clusters:**
  - **k=3:** Captura correctamente las tres especies principales (setosa, versicolor, virginica) con buena separación y dispersión interna razonable.
  - **k=4:** Se observan subvariantes internas dentro de versicolor/virginica, generando clusters más compactos, pero ya no coincide directamente con la clasificación biológica principal.
  - **k=6–8:** Fragmentación excesiva; los clusters pierden sentido biológico y solo reflejan divisiones matemáticas.

- **Interpretación:** k=3 equilibra homogeneidad interna y separación entre clusters, representando fielmente la estructura real del dataset y evitando fragmentaciones artificiales.

