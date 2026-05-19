# Simon Proa 2026

Juego Simon preparado para practicar trabajo colaborativo con **Git, GitHub y Visual Studio Code**.

## Objetivo

Trabajar en grupos sobre un mismo proyecto usando este flujo:

```text
clonar -> crear rama -> modificar -> commit -> push -> Pull Request -> merge -> pull
```

## Archivos principales

- `index.html`: estructura del juego.
- `styles.css`: estilos visuales.
- `game.js`: logica del juego.
- `sounds/`: sonidos del juego.

## Para probar el juego

Abrir `index.html` en el navegador.

Antes de modificar, verificar:

- la pagina carga
- los botones se ven
- el juego inicia
- la secuencia responde

## Trabajo en clase

Cada grupo trabaja en una rama propia y crea un Pull Request.

El docente revisa y hace merge a `main`.

Despues del merge, todos actualizan su copia:

```bash
git switch main
git pull origin main
```
