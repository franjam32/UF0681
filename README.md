# UF0681 · Autoevaluaciones

Conversión de los dos paquetes originales iSpring a una web HTML estática.
Conserva el reproductor, diseño, imágenes, preguntas, respuestas, puntuación y actividades originales. Se ha sustituido el inicio SCORM por el inicio autónomo del reproductor. No requiere Moodle ni una API SCORM.

## Subir a GitHub Pages

1. Descomprime el ZIP.
2. Sube TODO su contenido al repositorio `franjam32/UF0681`. El archivo `index.html` debe quedar en la raíz, junto con `actividad.html`, `preguntas` y `anatomia`.
3. En GitHub abre Settings → Pages → Deploy from a branch.
4. Selecciona la rama `main`, carpeta `/ (root)`, y guarda.
5. Cuando GitHub termine el despliegue, abre https://franjam32.github.io/UF0681/.

No subas solamente el ZIP ni solamente index.html: las carpetas contienen el reproductor, fuentes e imágenes necesarios.

## Uso

La portada permite elegir Preguntas (39 actividades) o Anatomía (15 ejercicios de arrastrar y soltar). “Inicio” vuelve al selector; “Ampliar” abre el bloque ocupando la pantalla. Se mantienen las opciones de corrección y repetición configuradas en cada original.

Los resultados no se envían al docente. El almacenamiento de estado que admite el reproductor depende del navegador; no se sincroniza entre dispositivos. No se han revisado ni modificado las respuestas médicas del material de origen.

Para una vista local fiable: `python3 -m http.server 8000` desde esta carpeta y abrir http://localhost:8000.
