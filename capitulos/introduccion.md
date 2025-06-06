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

### Innovación Metodológica

Inspirados por investigaciones recientes, particularmente el trabajo de Kieran Gibb publicado en Ecological Informatics, proponemos adaptar y aplicar autoencodificadores variacionales convolucionales (VAE) al estudio de nuestras especies locales. Esta metodología, que ha demostrado resultados prometedores en el estudio de vocalizaciones de aves, podría revolucionar nuestra capacidad para monitorear y comprender las poblaciones de anfibios en los humedales de la región.

### Desafíos Técnicos

Los paisajes sonoros naturales presentan desafíos únicos para el análisis automatizado. Las vocalizaciones de anfibios frecuentemente se encuentran inmersas en una matriz compleja de sonidos ambientales, desde la lluvia hasta el ruido urbano. La magnitud de datos generados en proyectos de monitoreo acústico —que pueden alcanzar terabytes por temporada— hace imperativa la implementación de soluciones automatizadas que no solo sean eficientes, sino también interpretables.

```{note}
Este capítulo introduce el trabajo de investigación sobre monitoreo acústico mediante VAE, estableciendo sus objetivos y alcance.
``` 