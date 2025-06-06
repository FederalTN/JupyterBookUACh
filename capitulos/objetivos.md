# Objetivos

## Objetivo General

Desarrollar y evaluar un modelo de VAE entrenado con datos locales que represente y clasifique vocalizaciones de anfibios en humedales urbano-naturales de Valdivia.

## Objetivos Específicos

1. Replicar el modelo VAE del paper de Gibb usando la base original de paisajes sonoros.

2. Entrenar el modelo con datos propios de anfibios y compararlo con redes de clasificación.

3. Evaluar la interpretabilidad y robustez de las representaciones latentes (p. ej., tolerancia al ruido).

4. Integrar el VAE en una herramienta de monitoreo.

## Pregunta de Investigación

¿Hasta qué punto un VAE puede discriminar especies de anfibios y, simultáneamente, ofrecer representaciones latentes interpretables que faciliten la detección de eventos raros?

## Hipótesis

Un VAE entrenado con espectrogramas Mel de anfibios generará un espacio latente donde muestras de la misma especie se agrupan de forma densa y separada de otras especies, incluso bajo condiciones de ruido de fondo variado.
