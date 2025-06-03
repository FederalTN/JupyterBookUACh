# Marco Teórico

## Monitoreo Acústico

El monitoreo acústico es una técnica que permite recopilar información sobre el entorno a través del análisis de señales sonoras. En el contexto de esta investigación, nos enfocamos en el desarrollo de sistemas automatizados para el procesamiento y análisis de estas señales.

## Autoencodificadores Variacionales (VAE)

Los Autoencodificadores Variacionales son una clase de modelos generativos que combinan redes neuronales con inferencia variacional. A diferencia de los autoencodificadores tradicionales, los VAE aprenden una distribución probabilística del espacio latente.

### Arquitectura del VAE

La arquitectura básica de un VAE consiste en:

1. **Encoder (q_φ(z|x))**: 
   - Codifica la entrada x en una distribución sobre el espacio latente
   - Produce los parámetros μ y σ de la distribución latente

2. **Espacio Latente**:
   - Distribución normal multivariada
   - Permite muestreo mediante el truco de reparametrización

3. **Decoder (p_θ(x|z))**:
   - Reconstruye los datos originales a partir de las muestras del espacio latente

## Procesamiento de Señales Acústicas

### Representación de Señales

Para el procesamiento de señales acústicas, utilizamos:

1. **Espectrogramas**:
   - Representación tiempo-frecuencia de la señal
   - Permite visualizar la evolución temporal del contenido frecuencial

2. **Transformada de Fourier de Tiempo Corto (STFT)**:
   - Análisis localizado de frecuencias
   - Base para la generación de espectrogramas

## Aplicaciones en Monitoreo Acústico

El monitoreo acústico automatizado tiene diversas aplicaciones:
- Detección de especies
- Análisis de biodiversidad
- Monitoreo ambiental
- Identificación de patrones acústicos

```{note}
Este capitulo se basa directamente en el contenido de mi tesis de investigación sobre monitoreo acústico mediante VAE.
``` 