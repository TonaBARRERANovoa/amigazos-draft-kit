# Amigazos Draft Kit

Cheat sheet de draft para la liga **Amigazos** (14 equipos, PPR completo).
Página estática de un solo archivo (`index.html`) — sin build, sin dependencias.

- **Board general** ordenado por VORP (valor sobre reemplazo) para una liga de 14.
- **Asistente de pick en vivo**: marca los picks conforme salen y recomienda a
  quién tomar con el motor real de Tona, precargado y portado a JavaScript:
  - proyección *blend* (mercado ECR × 0.55 + modelo × 0.45, curva calibrada
    con 2022–2025) menos el nivel de reemplazo derivado para 14 equipos;
  - recomendación por **necesidad de roster × VONA** con probabilidad de
    disponibilidad (ADP de ESPN), ajuste de corrida, penalización de choque de
    byes de la misma posición y desempate de calendario de playoffs;
  - excluye lesionados (Out / IR / Doubtful / suspensión).
  Todo corre en el navegador (`localStorage`); no necesita internet ni cuenta.

Datos: consenso FantasyPros al 6 de septiembre de 2026. Es una guía, no una regla.

Hecho por Tona Barrera · **TB · Fantasy**

## Ver / desplegar

HTML estático. Cualquier host sirve:
- **Local:** abre `index.html`.
- **GitHub Pages:** Settings → Pages → Source `main` / `/` (root).
- **Vercel:** [vercel.com/new](https://vercel.com/new) → importa este repo →
  preset **Other**, sin build command → Deploy.
