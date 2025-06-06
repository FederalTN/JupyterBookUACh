# Introducción

## Contexto y Motivación

El monitoreo acústico representa una ventana hacia la comprensión de nuestros ecosistemas naturales, especialmente en una era donde la recopilación masiva de datos ambientales se ha vuelto fundamental. Esta metodología permite capturar la riqueza sonora de los entornos naturales en todas sus dimensiones: desde las vocalizaciones de la fauna (biofonía), los sonidos naturales del ambiente (geofonía), hasta la influencia sonora humana (antropofonía).

La complejidad inherente de estos registros acústicos —donde múltiples fuentes sonoras se entrelazan en patrones intrincados— ha impulsado la búsqueda de soluciones innovadoras basadas en aprendizaje profundo. Estas herramientas computacionales prometen transformar la manera en que procesamos y entendemos los paisajes sonoros a gran escala.

### Enfoque en Anfibios de la Región de Los Ríos

Nuestra investigación se centra en un grupo particularmente fascinante y poco estudiado: los anfibios de la Región de Los Ríos. De las 63 especies de anfibios presentes en Chile, nuestra región alberga una proporción significativa, gracias a sus diversos ecosistemas de bosques templados y ambientes acuáticos. Estos organismos no solo representan una parte vital de nuestra biodiversidad local, sino que también actúan como sensibles bioindicadores de la salud ecosistémica.

```{figure} images/Valdivia-Zones-map.jpg
:name: mapa-valdivia
:align: center

Mapa de las zonas de estudio en la Región de Los Ríos
```

A diferencia de otros grupos taxonómicos como las aves, que cuentan con extensas bases de datos acústicos, los registros de vocalizaciones de anfibios permanecen relativamente escasos y fragmentados. Esta brecha en el conocimiento representa tanto un desafío como una oportunidad para la investigación.

```{figure} images/birds_results.png
:name: birds-global
:align: center
:width: 45%

Registros globales de vocalizaciones de aves
```

```{figure} images/amphibians_results.png
:name: amphibians-global
:align: center
:width: 45%

Registros globales de vocalizaciones de anfibios
```

```{figure} images/birds_chile_results.png
:name: birds-chile
:align: center
:width: 45%

Registros de vocalizaciones de aves en Chile
```

```{figure} images/amphibians_chile_results.png
:name: amphibians-chile
:align: center
:width: 45%

Registros de vocalizaciones de anfibios en Chile
```
## Monitoreo Acústico

El monitoreo acústico es una técnica que permite recopilar información sobre el entorno a través del análisis de señales sonoras. En el contexto de esta investigación, nos enfocamos en el desarrollo de sistemas automatizados para el procesamiento y análisis de estas señales.

```{audio} audios/soundscape_workshop.wav
:controls: true
:loop: false

## Autoencodificadores Variacionales (VAE)

Los Autoencodificadores Variacionales son una clase de modelos generativos que combinan redes neuronales con inferencia variacional. A diferencia de los autoencodificadores tradicionales, los VAE aprenden una distribución probabilística del espacio latente.

### Innovación Metodológica

Inspirados por investigaciones recientes, particularmente el trabajo de Kieran Gibb publicado en Ecological Informatics, proponemos adaptar y aplicar autoencodificadores variacionales convolucionales (VAE) al estudio de nuestras especies locales. Esta metodología, que ha demostrado resultados prometedores en el estudio de vocalizaciones de aves, podría revolucionar nuestra capacidad para monitorear y comprender las poblaciones de anfibios en los humedales de la región.


```{note}
Este capítulo introduce el trabajo de investigación sobre monitoreo acústico mediante VAE, estableciendo sus objetivos y alcance.
``` 