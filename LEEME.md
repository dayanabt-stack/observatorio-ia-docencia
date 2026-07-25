# Observatorio de IA para la Docencia — UTFSM (prototipo)

Este paquete trae el sitio completo, no solo el HTML: hoja de estilos y
script separados, más los archivos de marca oficial que nos compartieron,
para que el equipo tenga todo en un solo lugar.

```
observatorio-ia-docencia-sitio/
├── index.html                     ← página principal
├── css/
│   └── style.css                  ← todos los estilos del sitio
├── js/
│   └── script.js                  ← menú móvil y mensajes de "prototipo"
├── assets/
│   ├── logo-usm-blanco.svg        ← logo que usa el sitio (cabecera y pie)
│   └── marca-oficial/             ← archivos de marca tal como los enviaron
│       ├── logo-usm_blanco.svg
│       ├── Marca-Institucional-Vertical.ai
│       ├── version horizontal.ai
│       ├── version horizontal.pdf
│       └── version horizontal.png
└── LEEME.md                       ← este archivo
```

`index.html` carga `css/style.css` y `js/script.js` como archivos externos
(antes iban incrustados en el mismo HTML), así que cualquiera del equipo
puede abrir solo `style.css` para ajustar colores o espaciados sin tocar el
HTML. Los tres archivos deben mantenerse juntos, con esta misma estructura
de carpetas, para que el sitio funcione.

---

## Opción A — Ver el sitio en vivo en 2 minutos (sin cuenta)

1. Ir a **https://app.netlify.com/drop**
2. Arrastrar la **carpeta completa** `observatorio-ia-docencia-sitio`
   (no solo el `index.html`) sobre la página.
3. Netlify entrega una URL pública al instante, tipo
   `nombre-aleatorio.netlify.app`.
4. Para poder actualizar el sitio después, crear una cuenta gratuita en
   Netlify y "reclamar" el sitio (`Claim this site`) antes de cerrar la
   pestaña.
5. Para actualizar: se vuelve a arrastrar la carpeta completa al mismo
   proyecto.

**Cuándo usar esta opción:** para revisiones rápidas o mostrarlo a alguien
esta semana, mientras se decide algo más permanente.

---

## Opción B — Espacio de trabajo para editar en grupo (recomendada)

1. Crear un repositorio gratuito en **https://github.com** (por ejemplo
   `observatorio-ia-docencia`). Puede ser privado mientras se trabaja.
2. Subir **todo el contenido de esta carpeta** (manteniendo la estructura
   de subcarpetas `css/`, `js/`, `assets/`) a la raíz del repositorio.
3. Ir a **Settings → Pages**, y en "Build and deployment" elegir
   **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. GitHub entrega una URL pública tipo
   `https://usuario.github.io/observatorio-ia-docencia/`.
5. Invitar a las personas del grupo como **colaboradores** del repositorio
   (Settings → Collaborators). Pueden editar `index.html`, `css/style.css`
   o `js/script.js` directamente desde el navegador de GitHub, o clonar el
   repositorio y trabajar con Claude Code, VS Code, etc.
6. Cada cambio guardado ("commit") en `main` actualiza el sitio publicado
   en unos minutos.

**Cuándo usar esta opción:** para el trabajo real del grupo durante las
próximas semanas, y como base para entregar luego a la Dirección General
de Comunicaciones cuando se valide el resto de la marca.

---

## Antes de compartir el link con más gente

- El banner superior ("Prototipo") y las etiquetas "contenido de ejemplo"
  siguen ahí a propósito: avisan que falta contenido real y validación
  final. Quítalos solo cuando el sitio esté listo para salir del equipo.
- La carpeta `assets/marca-oficial/` no la usa el sitio directamente (el
  sitio solo usa `assets/logo-usm-blanco.svg`); está ahí como respaldo de
  los archivos de marca originales, útil si alguien necesita el logo en
  otro formato (.ai, .pdf) para materiales impresos.
- Los 5 colores institucionales están documentados arriba de `css/style.css`,
  en el bloque `:root`, por si hay que ajustarlos.
