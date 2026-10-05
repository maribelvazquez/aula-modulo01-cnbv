# Aula del Repaso · Módulo 1

Aula de 360Educa (GMC360) armada con `armar_aula.py` el 05/10/2026 · v3.

| Carpeta | Contenido |
|---|---|
| `index.html` | Portada: 10 temas, simulacro y biblioteca de 9 fuentes |
| `m1-s1-conceptos/` | S1 · Conceptos básicos (mapa) |
| `m1-s2-organismos/` | S2 · Organismos y GAFI (mapa) |
| `m1-s3-recomendaciones/` | S3 · Las 40 Recomendaciones (mapa) |
| `m1-s4-autoridades/` | S4 · Autoridades nacionales (mapa) |
| `m1-quien-hace-que/` | ¿Quién hace qué? · entrenador (externa) |
| `m1-simulacro/` | Simulacro mixto: 516 reactivos, S3 30 % · S2 27 % · S1 23 % · S4 20 % |

## Reactivos que no entraron al simulacro (con su motivo)
- G097: reforma jun-2026, fuera de la bibliografía
- G098: reforma jun-2026, fuera de la bibliografía
- G119: duplica O089
- G411: duplica O014/O015
- E011: duplica O078
- E013: duplica O088

## Cómo se corrige
- No se edita ningún `index.html` a mano. Se corrige la lección en su proyecto (su `datos.json`) y se vuelve a armar el aula con `armar_aula.py`.
- Las lecciones no verificadas no entran al simulacro: se declara en `aula.json` (`verificacion`).

## Cómo publicarlo
Netlify sin GitHub: app.netlify.com/drop y arrastra la carpeta con `index.html`. Las ligas internas son relativas.

Material didáctico: los textos están resumidos y no sustituyen la publicación oficial.
