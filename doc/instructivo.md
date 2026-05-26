# Instructivo Simon Proa 2026

## Objetivo

Hacer el primer trabajo colaborativo sobre este repositorio:

```text
clonar -> explorar -> probar -> crear rama -> modificar -> commit -> push -> Pull Request
```

Repositorio:

```text
https://github.com/lole-s/simon-proa-2026
```

---

## 1. Clonar el repositorio

Desde VS Code:

1. Abrir `Ctrl + Shift + P`.
2. Buscar `Git: Clone`.
3. Pegar:

```text
https://github.com/lole-s/simon-proa-2026.git
```

4. Elegir carpeta de trabajo.
5. Abrir el proyecto clonado.

Antes de crear una rama:

```bash
git switch main
git pull origin main
```

---

## 2. Explorar los archivos principales

Simon es un juego de memoria. La app muestra una secuencia de colores y sonidos. La persona que juega debe repetir esa secuencia en el mismo orden.

Archivos principales:

| Archivo o carpeta | Para que sirve |
|---|---|
| `index.html` | Estructura visible de la pagina. |
| `styles.css` | Colores, tamanios y estilos. |
| `game.js` | Logica del juego. |
| `sounds/` | Sonidos del juego. |
| `README.md` | Presentacion del proyecto. |
| `doc/` | Documentacion e instructivos. |
| `doc/grupos.md` | Registro de grupos e integrantes. |

Responder:

```text
¿Que archivo se abre en el navegador?
¿Que archivo cambia el aspecto visual?
¿Que archivo controla la logica del juego?
¿Donde estan los sonidos?
```

---

## 3. Abrir y probar la app

Abrir `index.html` en el navegador.

Desde VS Code:

1. Buscar `index.html`.
2. Clic derecho.
3. Elegir **Reveal in File Explorer** o **Mostrar en el Explorador de archivos**.
4. Abrirlo con doble clic.

Probar:

- si la pagina carga
- si se ven los botones de colores
- si el juego inicia
- si aparece una secuencia
- si los botones responden

Responder:

```text
¿De que se trata la app?
¿Que tiene que hacer la persona que juega?
¿Que pasa cuando acierta?
¿Que pasa cuando se equivoca?
¿El proyecto funciona antes de hacer cambios?
```

---

## 4. Organizar roles

Cada grupo tiene 3 integrantes.

| Rol | Responsabilidad |
|---|---|
| Coordinacion Git | Crea la rama, hace commit, push y abre el PR. |
| Desarrollo | Escribe la modificacion acordada. |
| Testing y registro | Prueba la app y completa las respuestas. |

Los tres integrantes revisan el cambio antes del commit y antes del Pull Request.

---

## 5. Tareas por grupo

Cada grupo crea la rama indicada y hace solo la modificacion asignada.

Todos los grupos deben agregar sus integrantes en `doc/grupos.md`.

| Grupo | Rama | Archivo principal | Tarea |
|---|---|---|---|
| 1 | `grupo-01-observacion-app` | `README.md` | Agregar una observacion sobre de que se trata la app. |
| 2 | `grupo-02-como-jugar` | `README.md` | Agregar una recomendacion breve para jugar por primera vez. |
| 3 | `grupo-03-prueba-juego` | `doc/instructivo.md` | Agregar una recomendacion para probar el juego antes de modificar. |
| 4 | `grupo-04-descripcion-simon` | `doc/simon-proa.md` | Mejorar la descripcion del juego con una frase clara. |
| 5 | `grupo-05-archivos-principales` | `README.md` | Agregar una aclaracion breve sobre algun archivo principal. |
| 6 | `grupo-06-testing` | `doc/instructivo.md` | Agregar una pregunta de testing para revisar la app. |
| 7 | `grupo-07-sonidos` | `doc/simon-proa.md` | Agregar una frase sobre el uso de sonidos en el juego. |
| 8 | `grupo-08-git-colaborativo` | `README.md` | Agregar una frase sobre por que este repo sirve para practicar Git. |

Ejemplo de cambio en `doc/grupos.md`:

```text
## Grupo 1

- Integrantes: Ana Perez, Juan Gomez, Sol Diaz
- Roles: Ana coordinacion Git, Juan desarrollo, Sol testing y registro
```

Ejemplo de cambio en el archivo principal:

```text
- Grupo 1: probamos la app y vimos que el juego consiste en repetir una secuencia de colores.
```

No modificar todavia `index.html`, `styles.css` ni `game.js`.

---

## 6. Crear la rama

Ejemplo para el grupo 1:

```bash
git switch -c grupo-01-observacion-app
```

Verificar:

```bash
git branch
```

---

## 7. Hacer la modificacion pequena

Modificar:

1. `doc/grupos.md`, para agregar integrantes y roles del grupo.
2. El archivo principal asignado en la tabla.

Antes de seguir:

- guardar los archivos
- revisar los cambios en VS Code
- verificar que el cambio sea pequeno y claro

---

## 8. Commit y push

Revisar primero los cambios:

```bash
git status
```

Hacer commit:

```bash
git add .
git commit -m "Agrego datos y observacion del grupo 1"
```

Subir la rama:

```bash
git push -u origin grupo-01-observacion-app
```

Cambiar el nombre de la rama y el mensaje segun el grupo.

---

## 9. Crear Pull Request

Un Pull Request es una propuesta para incorporar los cambios de una rama a `main`.

En GitHub:

1. Entrar al repositorio.
2. Buscar la rama publicada.
3. Hacer clic en **Compare & pull request**.
4. Completar:

```text
Grupo:
Integrantes:
Rama:
Archivos modificados:
Que cambiamos:
Como lo revisamos:
```

5. Crear el Pull Request.

Responder:

```text
¿Cual es el enlace al PR?
¿Desde que rama sale?
¿Hacia que rama quiere entrar?
¿Por que no modificamos main directamente?
```

---

## 10. Mostrar el PR al docente

Antes de terminar, mostrar:

- rama creada
- commit realizado
- push realizado
- Pull Request creado
- integrantes registrados en `doc/grupos.md`

---

## 11. Para entregar

```text
Grupo:
Integrantes:
Roles:
Rama:
Archivos modificados:
Cambio realizado:
Enlace al PR:
```

---

## Proxima clase

Vamos a recuperar la rama desde otra computadora y sincronizar cambios con GitHub.
