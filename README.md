# Detección de transformaciones de cobertura del suelo mediante U-Net

## Descripción general

Este proyecto tiene como objetivo desarrollar un modelo de inteligencia artificial basado en una red neuronal convolucional U-Net para la detección de transformaciones de la cobertura del suelo en la Cuchilla El Tablazo, ubicada en Subachoque, dentro del Complejo de Páramos Guerrero.

El modelo utiliza imágenes satelitales Sentinel-2 correspondientes a los años 2017 y 2024, junto con información espectral y datos de referencia, para realizar una segmentación de coberturas terrestres píxel por píxel. La red neuronal busca identificar categorías como vegetación natural de páramo, bosque y vegetación arbórea, pastos y áreas agropecuarias, suelo desnudo o intervenido y agua.

## Modelo de inteligencia artificial

El modelo utilizado corresponde a una arquitectura **U-Net**, una red neuronal convolucional diseñada para tareas de segmentación semántica de imágenes. Su función es analizar información espacial y espectral para asignar una clase de cobertura a cada píxel de la imagen de entrada.

## Datos utilizados

- Imágenes multiespectrales Sentinel-2.
- Bandas espectrales B2, B3, B4, B8, B11 y B12.
- Índices espectrales NDVI y NDMI.
- Etiquetas de cobertura terrestre.
- Parches de imágenes de 64x64 píxeles.
- Información complementaria del área de estudio.

## Área de estudio

El proyecto se desarrolla en la Cuchilla El Tablazo, Subachoque, perteneciente al Complejo de Páramos Guerrero y al Distrito Regional de Manejo Integrado Macizo El Tablazo.

## Ficha técnica del modelo

La información detallada del modelo, sus características, datos utilizados, proceso de entrenamiento, limitaciones y consideraciones de uso se encuentra en:

[Model Card - U-Net Tablazo](./MODEL_CARD.md)

## Autor de la ficha

**Nombre:** Danna Valentina Valbuena Robayo  
**Programa:** Ingeniería Catastral y Geodesia  
**Proyecto:** Detección de transformaciones de cobertura del suelo mediante IA  
**Fecha:** Octubre de 2026
