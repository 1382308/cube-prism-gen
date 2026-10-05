# Generador de prismas

**Demo:** https://1382308.github.io/cube-prism-gen/

Herramienta web para dibujar prismas rectangulares (opcionalmente divididos en cubos unitarios) en proyección oblicua, con estilo normal o "a mano", y exportarlos como PNG (fondo transparente), SVG o GIF animado.

![Captura](Screenshot.png)

## Uso

Abre `index.html` en el navegador. No necesita instalación ni servidor: todo (incluidas las librerías en `lib/`) está en el repositorio.

- **Ancho / Alto / Profundidad**: dimensiones del prisma (1–20).
- **Unidad**: mm, cm, dm, m o km.
- **Dibujar en cubos**: muestra la cuadrícula de cubos unitarios.
- **Estilo a mano**: trazo tipo boceto (Rough.js + Excalifont). Cada vez que se marca se genera un temblor distinto.
- **Letra central**: etiqueta opcional en el centro.
- **Barra superior (como Excalidraw)**: Trazo, Fondo (incluye transparente), Relleno (rayado, rayado cruzado, sólido, zigzag), Grosor del trazo, Estilo del trazo (continuo, discontinuo, punteado) y Descuido (arquitecto, artista, caricaturista).

## Exportar

- **PNG**: fondo transparente, siempre a ×4 (~1700 px de ancho).
- **SVG**: vectorial; la fuente va incrustada. El texto sigue siendo texto, por lo que Canva puede no mostrarlo igual; para Canva usa el PNG.
- **GIF animado** (solo con estilo a mano): el trazo se dibuja y después las líneas "hierven" (*line boil*). Fondo transparente, ×2.

## Créditos

- [Rough.js](https://roughjs.com/) (MIT)
- [Excalifont](https://github.com/excalidraw/excalidraw) (OFL)
- [gifenc](https://github.com/mattdesl/gifenc) (MIT)
