# Simon Proa 2026

Juego Simon preparado para practicar trabajo colaborativo con **Git, GitHub y Visual Studio Code**.

## Objetivo

Este repositorio se usa para aprender el flujo de trabajo colaborativo:

```text
clonar -> explorar -> crear rama -> modificar -> commit -> push -> Pull Request
```

En una clase posterior se trabaja cómo recuperar una rama desde otra computadora y cómo sincronizar `main` después de los merges.

## De qué se trata la app

Simon es un juego de memoria. La app muestra una secuencia de colores y sonidos. La persona que juega debe repetir esa secuencia en el mismo orden.

Si acierta, avanza de nivel y la secuencia se hace más larga. Si se equivoca, el juego muestra un error y se puede volver a empezar.

## Archivos principales

- `index.html`: estructura visible de la página.
- `styles.css`: estilos visuales, colores, tamaños y distribución.
- `game.js`: lógica del juego, secuencia, niveles y respuestas.
- `sounds/`: sonidos del juego.
- `doc/`: documentación e instructivos.
- `doc/grupos.md`: registro de grupos, integrantes y roles.
- `doc/actividad-2-modificar-juego.md`: actividad para modificar el juego y revisar el deploy.

## Para probar el juego

Abrir `index.html` en el navegador.

Antes de modificar, verificar:

- la página carga
- se ven los cuatro botones de colores
- el juego inicia
- la secuencia responde
- los botones tienen respuesta visual o sonora

Actividad breve:

```text
¿De qué se trata la app?
¿Qué tiene que hacer la persona que juega?
¿Qué archivo se abre en el navegador?
¿Qué archivo cambia el aspecto visual?
¿Qué archivo controla la lógica del juego?
```

## Trabajo en grupos

Cada grupo tiene 3 integrantes:

| Rol | Responsabilidad |
|---|---|
| Coordinación Git | Crea la rama, revisa cambios, hace commit, push y abre el Pull Request. |
| Desarrollo | Propone y escribe la modificación pequeña acordada por el grupo. |
| Testing y registro | Prueba la app, completa las respuestas y revisa que el PR explique el cambio. |

En esta primera actividad, cada grupo trabaja en una rama propia y crea un Pull Request con una modificación pequeña en la documentación.

El docente revisa los Pull Requests y decide cuándo hacer merge a `main`.

## Actividad 2

La segunda actividad propone modificar una parte pequeña del juego y ver el resultado publicado en Vercel:

```text
doc/actividad-2-modificar-juego.md
```

App publicada:

```text
https://simon-proa-2026.vercel.app/
```
