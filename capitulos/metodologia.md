```{note}
Este capitulo se basa directamente en el contenido de mi tesis de investigación sobre monitoreo acústico mediante VAE.
```

# Metodología general

Ahondemos ahora, como lograremos esto:

La metodología tiene tres etapas:

## 1. Revisión y replicación del modelo base

### Código y arquitectura VAE de referencia
Se toma como base el modelo propuesto por Gibb et al. (2024), que utiliza una arquitectura encoder–decoder convolucional profunda para aprender representaciones latentes de espectrogramas Mel.

### Base de datos de aves
Se emplean las grabaciones provistas en el trabajo original (4725 fragmentos de 1 minuto provenientes de sitios en el Reino Unido y Ecuador) con el fin de mantener la fidelidad al enfoque planteado por los autores.

### Configuración y entrenamiento inicial
- Preprocesamiento del audio (conversión a espectrogramas log-Mel y normalización).
- Entrenamiento del VAE mediante mini-batches, maximizando la evidencia ELBO (término de reconstrucción + término KL).
- Evaluación de la calidad de reconstrucción y la capacidad de diferenciación de hábitats (o especies) mediante técnicas de proyección (UMAP) y clasificadores sencillos (e.g., regresión logística).

## 2. Migración a la base de datos de anfibios

### Base de datos propia
Se dispone de grabaciones de anfibios cuidadosamente etiquetadas, obtenidas en humedales urbano-naturales de la región de Los Ríos. Estas incluyen especies como:
- Batrachyla leptopus
- Batrachyla taeniata
- Caliptocephalella gayi
- Pleurodema thaul
- Entre otras

### Entrenamiento desde cero
El mismo modelo VAE se entrena con estas grabaciones, ajustando hiperparámetros (por ejemplo, rangos de frecuencia) para adaptarse a las características acústicas de los llamados de anfibios.

### Transfer Learning
Paralelamente, se evalúa la posibilidad de partir del modelo entrenado con datos de aves (es decir, utilizando los pesos del encoder y decoder) y realizar un ajuste fino (fine-tuning) con la nueva base de datos de anfibios, con el objetivo de mejorar la eficiencia y la capacidad de generalización.

## 3. Comparación con otras redes neuronales

### Modelos CNN supervisados
Como línea base, se consideran arquitecturas clásicas de clasificación supervisada (redes convolucionales especializadas), entrenadas directamente con las etiquetas de especie de la base de datos de anfibios.

### Evaluación del VAE
Aunque el VAE es un modelo generativo, se pueden extraer sus vectores latentes y utilizarlos como entrada para clasificadores simples (como SVM o regresión logística), evaluando su exactitud y F1-score en la identificación de especies.

### Interpretabilidad
Se analiza la interpretabilidad de las representaciones latentes del VAE en comparación con las de modelos puramente supervisados. El objetivo es determinar la utilidad de los espacios latentes para identificar claramente las diferencias entre especies y detectar eventos poco frecuentes. 