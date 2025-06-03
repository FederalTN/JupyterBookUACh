# Metodología

## Diseño del Sistema

### Arquitectura del VAE

La arquitectura del sistema se compone de:

1. **Preprocesamiento de Señales**
   - Conversión a espectrogramas
   - Normalización de datos
   - Segmentación de señales

2. **Estructura del Encoder**
   - Capas convolucionales
   - Capas densas
   - Capa de muestreo del espacio latente

3. **Estructura del Decoder**
   - Capas deconvolucionales
   - Capas densas
   - Capa de reconstrucción

## Implementación

### Preprocesamiento de Datos

```python
def preprocess_audio(audio_file):
    # Código de ejemplo para el preprocesamiento
    signal, sr = librosa.load(audio_file)
    spectrogram = librosa.feature.melspectrogram(y=signal, sr=sr)
    return spectrogram
```

### Entrenamiento del Modelo

El proceso de entrenamiento incluye:
1. Carga y preprocesamiento de datos
2. Definición de hiperparámetros
3. Entrenamiento del VAE
4. Validación del modelo

## Evaluación

### Métricas de Evaluación

- Error de reconstrucción
- Divergencia KL
- Precisión en la detección
- F1-score

### Protocolo de Pruebas

Descripción detallada del protocolo de pruebas utilizado para evaluar el sistema.

```{note}
Este capitulo se basa directamente en el contenido de mi tesis de investigación sobre monitoreo acústico mediante VAE.
``` 