# Sonificacion-imagenes

# Sonificador de Imágenes

Herramienta interactiva que convierte datos visuales en sonido mediante el mapeo directo de valores de píxeles a frecuencias sintetizadas.

## Descripción
Exploración de la relación entre datos visuales y datos acústicos. La herramienta lee la matriz de píxeles de una imagen (RGB y brillo) y mapea dichos valores numéricos hacia parámetros de síntesis de audio (frecuencia, tono y amplitud), generando un paisaje sonoro representativo de la imagen.

## Tecnologías y Herramientas
* **p5.js:** Carga, procesamiento numérico y lectura de píxeles del lienzo.
* **Web Audio API (p5.sound):** Osciladores y generadores de tono para síntesis en tiempo real.
* **JavaScript:** Lógica de mapeo matemáticamente proporcional entre espacio de color y espacio de frecuencia.

## Uso
1. Cargar una imagen en el lienzo o interactuar con el puntero sobre la imagen activa.
2. Analizar el tono y espectro sonoro resultante según las coordenadas e intensidad cromática.
