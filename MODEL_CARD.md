# Model Card: U-Net para segmentación de coberturas terrestres en la Cuchilla El Tablazo

## 1. Información del modelo

**Nombre del modelo:**  
U-Net para detección de transformaciones de cobertura del suelo

**Versión:**  
1.0

**Fecha de creación:**  
Octubre de 2026

**Autor de la ficha:**  
Danna Valentina Valbuena Robayo

**Tipo de modelo:**  
Red neuronal convolucional (CNN) especializada en segmentación semántica de imágenes.

**Tarea principal:**  
Clasificación de coberturas terrestres píxel por píxel mediante imágenes satelitales.

---

## 2. Descripción general del modelo

El modelo U-Net corresponde a una arquitectura de red neuronal convolucional diseñada para tareas de segmentación semántica de imágenes. Su objetivo dentro del proyecto es analizar información espacial y espectral para identificar diferentes tipos de cobertura del suelo en la Cuchilla El Tablazo, ubicada en Subachoque, dentro del Complejo de Páramos Guerrero.

El modelo busca detectar transformaciones de la cobertura terrestre entre los años 2017 y 2024 mediante el análisis de imágenes satelitales Sentinel-2.

---

## 3. Uso previsto

El modelo está diseñado para apoyar procesos de análisis territorial y ambiental mediante la identificación automática de coberturas terrestres.

Las aplicaciones previstas incluyen:

- Detección de cambios en la cobertura del suelo.
- Generación de mapas de cobertura terrestre.
- Apoyo al monitoreo de ecosistemas estratégicos.
- Análisis espacial del territorio.

---

## 4. Datos utilizados

El modelo utiliza información geoespacial y datos satelitales correspondientes al área de estudio.

Los datos considerados son:

- Imágenes multiespectrales Sentinel-2 de los años 2017 y 2024.
- Bandas espectrales B2, B3, B4, B8, B11 y B12.
- Índices espectrales NDVI y NDMI.
- Etiquetas de cobertura terrestre.
- Parches de imágenes de 64x64 píxeles.
- Información complementaria como elevación, pendiente, vías, zonas agropecuarias y senderos.

---

## 5. Área de aplicación

El modelo se aplica en la Cuchilla El Tablazo, ubicada en el municipio de Subachoque, dentro del Complejo de Páramos Guerrero y el Distrito Regional de Manejo Integrado Macizo El Tablazo.

---

## 6. Arquitectura del modelo

La arquitectura U-Net está compuesta por:

- **Codificador:** extrae características espaciales y espectrales de la imagen.
- **Cuello de botella:** resume la información aprendida por la red.
- **Decodificador:** recupera la información espacial para generar la segmentación.
- **Conexiones de salto:** conservan detalles importantes de la imagen original.

El resultado final corresponde a un mapa clasificado donde cada píxel recibe una categoría de cobertura.

---

## 7. Clases de cobertura identificadas

El modelo busca reconocer las siguientes categorías:

- Vegetación natural de páramo.
- Bosque y vegetación arbórea.
- Pastos y áreas agropecuarias.
- Suelo desnudo o intervenido.
- Agua.

---

## 8. Entrenamiento del modelo

El entrenamiento del modelo se realizará utilizando imágenes procesadas, etiquetas de cobertura y parches de entrenamiento de 64x64 píxeles.

El modelo aprenderá patrones espectrales y espaciales presentes en las imágenes satelitales para realizar la clasificación automática de coberturas.

---

## 9. Evaluación del modelo

La evaluación del modelo se realizará mediante métricas de desempeño para modelos de segmentación semántica.

Las métricas consideradas incluyen:

- Exactitud de clasificación.
- Precisión.
- Recall.
- Intersección sobre Unión (IoU).

Los valores finales dependerán del proceso de entrenamiento y validación del modelo.

---

## 10. Limitaciones

El modelo puede presentar limitaciones relacionadas con:

- Calidad y disponibilidad de las imágenes satelitales.
- Similitud espectral entre diferentes coberturas.
- Cantidad y calidad de las muestras utilizadas para entrenamiento.
- Necesidad de validación mediante información de referencia.

Los resultados del modelo deben ser interpretados como apoyo al análisis territorial y no como sustituto del criterio de expertos.

---

## 11. Consideraciones éticas

El uso del modelo debe considerar:

- Transparencia sobre sus capacidades y limitaciones.
- Uso responsable de información geoespacial.
- Validación humana antes de tomar decisiones ambientales o territoriales.
- Reconocimiento de posibles errores de clasificación.
