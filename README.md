# TemiusKin

Temas de toda la app para [Kino](https://kinotvapp.github.io/kino-plugins/): no reproduce
nada, no se conecta a internet, y solo ofrece looks en **Ajustes ▸ Apariencia**.
Requiere **Kino 0.9.87 o más nuevo** (apiVersion 26).

Instálalo desde Plugins ▸ Agregar con:

```
Lenoxlkz/TemiusKin
```

## Los 8 temas

### AMOLED
- **AMOLED Puro** — negro puro (#000000 en fondo y tarjetas), acento violeta ajustable
  (cian, naranja, azul o rojo) y sombras apagadas. Pensado para paneles OLED.

### Material You
Colores tonales oscuros tipo Material You, esquinas expresivas y botones en pastilla.
Accento, radios, tamaño del texto y fondo ajustables en Apariencia ▸ Personalizar.
- **Material Azul** · **Material Verde** · **Material Arena**

### Liquid Glass
Brillos degradados, contornos con reflejo, resplandores suaves, hérore enmarcado y
riel flotante (los dos últimos solo en TV). Se activan con la experiencia visual completa.
- **Glass Medianoche** · **Glass Esmeralda** · **Glass Amatista** · **Glass Obsidiana**

## Notas técnicas

- Los temas son puros datos del manifiesto (`appThemes`): sin código, sin red, sin permisos.
- Liquid Glass usa las llaves de apiVersion 26 (`surfaces`, `style.gloss`, `layout`,
  `shape.heroRadius`, `shape.railItemRadius`); AMOLED y Material You son de nivel 1 y
  funcionan igual en cualquier Kino que acepte el manifiesto.
- Todo tema se ve bien con los siete efectos apagados: los efectos solo suman.
- Para validar en local: `node sdk/validate.mjs .`
