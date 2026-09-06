# Sonificacion-imagenes

# Sonificador RGB

Repositorio de sonificación visual e interacción sonora en tiempo real. Este proyecto consiste en una aplicación web interactiva que traduce la información cromática de archivos de imagen en síntesis musical mediante el análisis de píxeles y el procesamiento de la Web Audio API.

---

## Características Principal del Proyecto

### Sonificador RGB Interactivo (Web App)
Aplicación web que analiza la matriz de píxeles de una imagen columna por columna para generar patrones melódicos y modular parámetros de audio en tiempo real con **Tone.js**.

* **Mapeo de Píxeles a Audio:**
  * **Canal Rojo (R):** Determina la altura de la nota (pitch) seleccionando la frecuencia dentro de la escala musical activa.
  * **Canal Verde (G):** Modula la dinámica, la amplitud y el volumen del sintetizador.
  * **Canal Azul (B):** Controla el nivel de mezcla y la profundidad del efecto espacial Chorus.
* **Rueda de Quintas SVG:** Interfaz vectorial interactiva para seleccionar la tonalidad y el modo (Mayor o Menor), reorganizando la escala sonora en tiempo real.
* **Algoritmo de Auto-Crop:** Detecta y elimina automáticamente los bordes o marcos negros de las imágenes antes de procesar el análisis de color.
* **Cadena de Procesamiento DSP:** Sintetizador con oscilador triangular, filtro Low-Pass, Chorus, Reverb y control de ganancia maestro.

---

## Tecnologías Utilizadas

* **Lenguajes:** JavaScript (ES6+), HTML5 Canvas, SVG Vectorial, CSS3 (Grid & CSS Variables).
* **Librerías de Audio:** Tone.js (Framework sobre la Web Audio API).

---

## Instrucciones de Uso

### Despliegue y Ejecución
1. Ingresa a la versión publicada mediante **GitHub Pages** o abre directamente el archivo `index.html` en el navegador.
2. Si ejecutas el proyecto localmente, es recomendable utilizar la extensión **Live Server** en VS Code para garantizar los permisos de lectura de imagen y evitar bloqueos del navegador.

### Flujo de Trabajo
1. Haz clic en **Cargar Imagen Local** para subir un archivo propio, o selecciona cualquiera de las **Imágenes de Prueba** (`JjAaZz`, `Abstract`, `Rug`).
2. Define la tonalidad inicial haciendo clic en los sectores de la **Rueda de Quintas**.
3. Presiona **▶ Iniciar Sonificación** para comenzar el escaneo visual de la línea y la generación de audio.
4. Ajusta los parámetros de **Filtro LPF**, **Reverb** y **Ganancia General** desde el panel lateral durante la reproducción.
