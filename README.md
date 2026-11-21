# TemiusKin

Temas de toda la app para [Kino](https://kinotvapp.github.io/kino-plugins/): no reproduce
nada, no se conecta a internet, y solo ofrece looks en **Ajustes ▸ Apariencia**.
Requiere **Kino 0.9.87 o más nuevo** (apiVersion 26).

Instálalo desde Plugins ▸ Agregar con:

```
Lenoxlkz/TemiusKin
```

## Fieles a su concepto (v1.2)

### AMOLED Puro — píxeles apagados
Negro verdadero `#000000` en fondo, tarjetas, panel del riel y placeholders (los huesitos
de carga no gastan píxeles). Sin sombras (0), sin resplandores, `heroScrim` al máximo,
movimiento mínima (crossfade 150 ms, sin zoom de foco ni drift): la paleta que menos
energía gasta en un panel OLED. Bordes hairline `#202020`, blanco puro para el texto.

### Material Azul / Verde / Arena — tonal system de Material You
Cada rol de color lleva el matiz de su semilla (estilo M3 dark): superficie contenedora,
superficie alta y panel del riel al tono, textos blanco roto teñidos, `outline` gris del
mismo tono. Elevación tonal (sombras suaves 0.3–0.42), formas expresivas (botones
pastilla 28, diálogos 28), título 1.08×, play circular 1.2× y drift del héroe.

### Glass Medianoche / Esmeralda / Amatista / Obsidiana — vidrio de verdad
Cada tema trae su **wallpaper abstracto** (`assets/wallpapers/`, generado sin banding,
~100–140 KB) detrás de toda la app con `dim 0.35`: el vidrio necesita algo que refractar.
`style.gloss` 0.8 para brillo especular, botones con relleno degradado + contorno
reflejo (degradado de stroke) + resplandor, `navActive` con halo, tarjetas enfocadas con
anillo claro + glow suave, héroe enmarcado y riel flotante en TV, y **fuente propia**
Space Grotesk (SIL OFL) en toda la app. `focusZoom` 1.1 y crossfade 360 ms para el
sensación pesada y fluida del vidrio.

## Notas técnicas

- Los temas son puros datos del manifiesto (`appThemes`): sin código, sin red, sin permisos.
- Assets (1 fuente + 4 wallpapers, 621 KB en total, 5 archivos de 16): Kino los descarga
  en la instalación desde este repositorio, verifica sha256 y bytes, y si alguno falla
  vuelve al color/fuente de Kino sin romper nada.
- Todo tema se ve bien con los siete efectos apagados: los efectos solo suman.
- En TV, las esquinas redondeadas siguen el interruptor del aparato (apagado por omisión).
- Validar en local: `node sdk/validate.mjs .`
