# TemiusKin

Temas de toda la app para [Kino](https://kinotvapp.github.io/kino-plugins/): no reproduce
nada, no se conecta a internet, y solo ofrece looks en **Ajustes ▸ Apariencia**.
Requiere **Kino 0.9.87 o más nuevo** (apiVersion 26).

Instálalo desde Plugins ▸ Agregar con:

```
Lenoxlkz/TemiusKin
```

## Qué cambia con cada tema (v1.1)

Cada tema no solo trae un acento: **tiñe el fondo con degradado, las tarjetas, los
paneles, los textos y los bordes**, y ajusta esquinas, sombras, movimiento, escalas
tipográficas y los controles del reproductor, como los mejores temas de la comunidad.

### AMOLED
- **AMOLED Puro** — negro de verdad (#000000 en fondo y tarjetas), bordes finos
  grises, acento violeta ajustable (cian, naranja, azul o rojo).

### Material You
Colores tonales oscuros tipo M3 (fondo y superficies con matiz del acento), bordes
visibles, botones en pastilla (radius 28), botón de play circular más grande y
drift del héroe. Accento, radios, tamaño del texto y fondo ajustables.
- **Material Azul** · **Material Verde** · **Material Arena**

### Liquid Glass
Además de lo anterior, usa las llaves de nivel 2 (apiVersion 26): **fuente
propia** (Space Grotesk, SIL OFL) en toda la app, botones con relleno degradado y
contorno-reflejo, resplandores suaves en tarjetas y foco, hérore enmarcado y riel
flotante en TV, y experiencia visual completa.
- **Glass Medianoche** (azul) · **Glass Esmeralda** (verde) · **Glass Amatista**
  (violeta) · **Glass Obsidiana** (pizarra)

## Notas técnicas

- Los temas son puros datos del manifiesto (`appThemes`): sin código, sin red, sin permisos.
- La fuente (`assets/fonts/SpaceGrotesk.ttf`, 137 KB) se descarga en la instalación
  desde este mismo repositorio y Kino comprueba su sha256; si no se lee, vuelve a la
  fuente de Kino sin fallar.
- Todo tema se ve bien con los siete efectos apagados: los efectos solo suman.
- En TV, las esquinas redondeadas siguen el interruptor del aparato (apagado por omisión).
- Validar en local: `node sdk/validate.mjs .`
