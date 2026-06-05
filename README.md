# Dots & Boxes - Sandbox Edition 🎲✏️

¡Bienvenido al tablero digital libre de **Dots and Boxes** (también conocido como *Timbiriche* o el *Juego de los cuadraditos*)! 

Este proyecto está diseñado bajo el enfoque **Vibe-Coding**: el script funciona como un tablero inteligente, interactivo y limpio, pero no impone reglas rígidas. La lógica del juego (el orden de los turnos, quién sumó un punto y el conteo final) la llevan los propios jugadores de forma honesta, recreando perfectamente la experiencia clásica de jugar con lápiz y papel.

## 🚀 Características
*   **Formato Sandbox Completo:** ¿Alguien se equivocó de arista? ¿Marcaste una línea sin querer? No pasa nada, podés desmarcarla con otro click al instante.
*   **Rotación Dinámica de Cajas:** Al hacer click en el interior de un cuadrado, este cambia cíclicamente: `Vacío ➔ Naranja ➔ Violeta ➔ Vacío`.
*   **Hitboxes Optimizados para Móviles:** Las áreas táctiles de las líneas son más anchas que el elemento visual, lo que permite jugar cómodamente en pantallas táctiles sin sufrir por falsos clicks.
*   **Diseño Moderno:** Interfaz responsiva y minimalista utilizando **Tailwind CSS**, ideal para jugar desde el celular o la computadora compartiendo pantalla.

## 🛠️ Estructura del Proyecto
El juego entero se resuelve de forma elegante en un único archivo autónomo:
*   `index.html`: Contiene la estructura semántica, los estilos embebidos (Tailwind + CSS nativo) y la lógica de manipulación del DOM mediante JavaScript.

## 📦 Despliegue rápido en GitHub Pages
Para publicar este tablero en tu propio sitio web gratis en menos de un minuto, seguí estos pasos:

1.  **Creá un repositorio en GitHub:** Dale un nombre descriptivo, por ejemplo, `dots-and-boxes`.
2.  **Subí el archivo:** Añadí el archivo `index.html` en la raíz (`root`) del repositorio.
3.  **Activá GitHub Pages:**
    *   Andá a la pestaña **Settings** (Configuración) de tu repositorio.
    *   En el menú izquierdo, hacé click en **Pages**.
    *   En la sección *Build and deployment*, seleccioná la rama `main` (o `master`) y la carpeta `/ (root)`.
    *   Hacé click en **Save**.
4.  **¡A jugar!** GitHub te dará un enlace público similar a `https://tu-usuario.github.io/dots-and-boxes/` listo para compartir.

## 🎮 Reglas del Juego Clásico
1.  El tablero consiste en una grilla de puntos de 6x6 (que forman 25 cajas de 1x1).
2.  En su turno, cada jugador dibuja una línea horizontal o vertical que une dos puntos adyacentes.
3.  Si un jugador cierra el cuarto lado de una caja de 1x1, esa caja le pertenece (la marca con su color) y **gana el derecho a un turno extra inmediato**.
4.  El juego termina cuando todas las líneas están hechas. ¡Gana quien tenga más cajas de su color!
