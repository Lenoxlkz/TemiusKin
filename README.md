# TemiusKin

Temas de toda la app para [Kino](https://kinotvapp.github.io/kino-plugins/): no reproduce
nada, no se conecta a internet, y solo ofrece looks en **Ajustes ▸ Apariencia**.
Requiere **Kino 0.9.87 o más nuevo** (apiVersion 26).

Instálalo desde Plugins ▸ Agregar con:

```
Lenoxlkz/TemiusKin
```

## Fieles a su concepto, a máxima potencia (v1.3)

### AMOLED Puro — píxeles apagados
Negro verdadero `#000000` en fondo, tarjetas, riel, scrim y placeholders de carga.
Cero sombras, cero resplandores, `focusZoom` 1.0, `heroDrift` off, crossfade 150 ms:
la configuración que menos energía gasta en OLED. Bordes hairline `#202020`,
estado con éxito/aviso/error/favoritos calibrados para negro (`#4ADE80`, `#FBBF24`,
`#FF453A`, `#FF2D55`).

### Material Azul / Verde / Arena — tonal system de Material You
Expresividad M3 subida: tarjetas 20, chips 24, inputs 16, botones pastilla 28,
diálogos 28. Toda la superficie al tono de la semilla, sombras tonales bajas,
título 1.08×, play circular 1.22×, drift del héroe y crossfade 280 ms.

### Glass Medianoche / Esmeralda / Amatista / Obsidiana — el mostrar completo
- **Wallpaper 1280×800 generado por tema**: aurora de dos tonos + haz diagonal de
  luz + núcleo especular + viñeta, sin banding, detrás de toda la app (`dim 0.3`).
- `style.gloss` 0.9 (brillo especular casi al tope).
- Resplandores fuertes: `navActive` con halo 12 dp α0.6, tarjetas enfocadas con
  anillo 2.5 dp y glow 18 dp, botones con degradado + stroke-reflejo + glow.
- **Gema de vidrio como logo**: anillo squircle con gema al acento en el riel de TV.
- `pluginColors "override"`: ni un plugin ajeno rompe la inmersión del vidrio.
- Fuente Space Grotesk (SIL OFL) en toda la app, héroe enmarcado, riel flotante,
  `focusZoom` 1.1, crossfade 380 ms.

## Notas técnicas

- Los temas son puros datos del manifiesto (`appThemes`): sin código, sin red, sin permisos.
- Assets: 1 fuente + 4 wallpapers (~1.4 MB en total, 5 de 16 archivos, tope 6 MB).
  Kino los descarga en la instalación desde este repositorio y verifica sha256 y bytes;
  si un asset falla, se usa el color/fuente de Kino y nada se rompe.
- Todo tema se ve bien con los siete efectos apagados: los efectos solo suman.
- En TV, las esquinas redondeadas siguen el interruptor del aparato (apagado por omisión).
- Validar en local: `node sdk/validate.mjs .`
