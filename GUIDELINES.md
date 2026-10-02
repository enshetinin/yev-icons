# Guidelines

Reglas que siguen todos los iconos. El build valida las que se pueden comprobar automáticamente (marcadas con ✓).

## Lienzo

- ✓ `viewBox="0 0 24 24"`.
- Margen de seguridad de 2px: el dibujo vive entre 2 y 22 en ambos ejes. Las formas grandes (círculos, documentos) llegan hasta 3–21.
- Coordenadas en enteros o medios píxeles para que el trazo quede nítido a 24px.

## Trazo

- ✓ `fill="none"` y `stroke="currentColor"` en la raíz. Nada de colores fijos.
- ✓ `stroke-width="1.5"`.
- ✓ `stroke-linecap="square"` y `stroke-linejoin="miter"`: esquinas y extremos rectos, sin redondeos.
- Los puntos (la “i” de info, el agujero de la etiqueta) se dibujan como un segmento de `.01` (`h.01`): con el extremo cuadrado se ven como un cuadrado de 1.5px.

## Estructura

- ✓ Solo formas planas autocerradas (`<path/>`, `<circle/>`, `<rect/>`…). Sin `<g>`, `<text>`, `<style>`, máscaras ni filtros.
- Mejor un único `<path>` por icono.

## Nombres

- ✓ Inglés, minúsculas, kebab-case: `arrow-left`, `external-link`.
- Nombra lo que el icono **muestra**, no dónde se usa: `plus`, no `add-post`.
- Las variantes de dirección van como sufijo: `arrow-up`, `arrow-up-right`, `chevron-right`.
- El componente React se deriva del nombre: `external-link` → `ExternalLinkIcon`.
