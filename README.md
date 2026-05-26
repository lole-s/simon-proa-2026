# Simon Proa 2026

Juego Simon preparado para practicar trabajo colaborativo con **Git, GitHub y Visual Studio Code**.

## Objetivo

Este repositorio se usa para aprender el flujo de trabajo colaborativo:

```text
clonar -> explorar -> crear rama -> modificar -> commit -> push -> Pull Request
```

En una clase posterior se trabaja como recuperar una rama desde otra computadora y como sincronizar `main` despues de los merges.

## De que se trata la app

Simon es un juego de memoria. La app muestra una secuencia de colores y sonidos. La persona que juega debe repetir esa secuencia en el mismo orden.

Si acierta, avanza de nivel y la secuencia se hace mas larga. Si se equivoca, el juego muestra un error y se puede volver a empezar.

## Archivos principales

- `index.html`: estructura visible de la pagina.
- `styles.css`: estilos visuales, colores, tamanios y distribucion.
- `game.js`: logica del juego, secuencia, niveles y respuestas.
- `sounds/`: sonidos del juego.
- `doc/`: documentacion e instructivos.
- `doc/grupos.md`: registro de grupos, integrantes y roles.

## Para probar el juego

Abrir `index.html` en el navegador.

Antes de modificar, verificar:

- la pagina carga
- se ven los cuatro botones de colores
- el juego inicia
- la secuencia responde
- los botones tienen respuesta visual o sonora

Actividad breve:

```text
¿De que se trata la app?
¿Que tiene que hacer la persona que juega?
¿Que archivo se abre en el navegador?
¿Que archivo cambia el aspecto visual?
¿Que archivo controla la logica del juego?
```

## Trabajo en grupos

Cada grupo tiene 3 integrantes:

| Rol | Responsabilidad |
|---|---|
| Coordinacion Git | Crea la rama, revisa cambios, hace commit, push y abre el Pull Request. |
| Desarrollo | Propone y escribe la modificacion pequena acordada por el grupo. |
| Testing y registro | Prueba la app, completa las respuestas y revisa que el PR explique el cambio. |

En esta primera actividad, cada grupo trabaja en una rama propia y crea un Pull Request con una modificacion pequena en la documentacion.

El docente revisa los Pull Requests y decide cuando hacer merge a `main`.
