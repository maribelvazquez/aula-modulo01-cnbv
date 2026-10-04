# Aula del Repaso · Módulo 1 · sitio v2

Sitio de estudio de 360Educa (GMC360) para el **Área 1 del temario CNBV PLD/FT de agosto de 2026**: conceptos y penas, organismos internacionales y autoridades nacionales. Ruta Sector financiero. Armado el 3-oct-2026. La v2 integra la Sesión 4; la v1 tenía la S4 como «Próximamente».

## Qué hay en esta carpeta

| Carpeta o archivo | Qué es |
|---|---|
| `index.html` | **Portada** («Aula del Repaso · Módulo 1», mismo formato que el Módulo 3). Trae los 10 temas del Área 1 (cada uno abre su sesión en la sección del tema), el simulacro mixto y la biblioteca de las 9 fuentes del temario con su liga oficial. |
| `m1-s1-conceptos/` | **Sesión 1 · Conceptos básicos** (1.1.1 a 1.1.5): LD y sus etapas, FT, corrupción y penas del CPF. 90 reactivos (C001–C090). |
| `m1-s2-organismos/` | **Sesión 2 · Organismos y GAFI** (1.2.1 y 1.2.2): ONU, Basilea, Wolfsberg, Egmont, GAFI, GAFILAT, las resoluciones 1267, 1373 y 1540, los órganos del GAFI y sus calificaciones. 90 reactivos (O001–O090). |
| `m1-s3-recomendaciones/` | **Sesión 3 · Las 40 Recomendaciones** (1.2.3): la app de Maribel, integrada sin cambiar su contenido. Sólo cambian la etiqueta («Módulo 1»), la ruta (financiera) y tres explicaciones corregidas. 262 reactivos (G…, E…). |
| `m1-s4-autoridades/` | **Sesión 4 · Autoridades nacionales** (1.3.1 y 1.3.2): el régimen de prevención y sus participantes, la UIF (art. 10 RISHCP) y la CNBV (Reglamento Interior). 80 reactivos (A001–A080). |
| `m1-simulacro/` | **Simulacro mixto**: sólo el simulador, con los bancos de las cuatro sesiones y sus ids originales. Ver «El simulacro mixto», abajo. |
| `LEEME.md` | Este archivo. |

Cada sesión y el simulacro traen arriba una franja negra:
- «Módulo 1» regresa a la portada.
- Los números 1 a 4 saltan entre sesiones.
- «Simulacro mixto» abre el simulador.

## El simulacro mixto

- **Reparto fijo por sesión:** S3 30 % · S2 27 % · S1 23 % · S4 20 %.
  - Un simulacro de 30 sale con 9 · 8 · 7 · 6 reactivos.
  - Un simulacro de 50 sale con 15 · 13 · 12 · 10.
- **Banco:** 516 reactivos.
- **Reactivos excluidos (sólo del mixto; siguen en la app de la S3):**
  - Cuatro de la S3 que duplican a la S2: E011, G119, G411 y E013.
  - Dos de la S3 que vienen de la reforma de junio de 2026 y no están en la bibliografía: G097 y G098.

## Cómo publicarlo en Netlify

- **Sin GitHub:**
  1. Entra a app.netlify.com/drop.
  2. Arrastra la carpeta descomprimida, la que tiene `index.html` y las carpetas `m1-…`.
- **GitHub + Netlify:**
  1. Sube todo a la raíz del repositorio `modulo1-cnbv`.
  2. En Netlify: Add new site → Import from GitHub, sin «Build command» ni «Publish directory».
  3. Cada vez que reemplaces los archivos, Netlify publica solo.
- Las ligas entre páginas son relativas: funcionan igual en Netlify, en la vista del artifact y abriendo los archivos desde una carpeta.

## Cómo se corrige

- **Sesiones y simulacro:**
  - No se edita ningún `index.html` a mano.
  - Se corrige el `datos.json` de la sesión, que está guardado en el proyecto de Claude «MÓDULO 1».
  - Después se vuelve a armar con `construir_modulo1.py` (documento «Módulo 1 · construir_modulo1 · v1» del mismo proyecto) y la plantilla «Plantilla Mapa Interactivo 360Educa».
- **Portada:** es un HTML propio, como la del Módulo 3. Sus textos y ligas están en los bloques `LIGAS`, `GRUPOS` y `FUENTES` de su script.

## Aviso

- Material didáctico: los textos están resumidos y no sustituyen la publicación oficial ni son asesoría para un caso concreto.
- El avance de cada simulador se guarda sólo en el navegador de quien estudia. Las claves son m1s1, m1s2, gafi40, m1s4 y m1mix.
