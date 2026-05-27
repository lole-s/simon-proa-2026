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

| Archivo o carpeta | Para qué sirve |
|---|---|
| `index.html` | Estructura visible de la página. |
| `styles.css` | Colores, tamaños y estilos. |
| `game.js` | Lógica del juego. |
| `sounds/` | Sonidos del juego. |
| `README.md` | Presentación del proyecto. |
| `doc/` | Documentación e instructivos. |
| `doc/grupos.md` | Registro de grupos e integrantes. |

Responder:

```text
¿Qué archivo se abre en el navegador?
¿Qué archivo cambia el aspecto visual?
¿Qué archivo controla la lógica del juego?
¿Dónde están los sonidos?
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

- si la página carga
- si se ven los botones de colores
- si el juego inicia
- si aparece una secuencia
- si los botones responden

Responder:

```text
¿De qué se trata la app?
¿Qué tiene que hacer la persona que juega?
¿Qué pasa cuando acierta?
¿Qué pasa cuando se equivoca?
¿El proyecto funciona antes de hacer cambios?
```

---

## 4. Organizar roles

Cada grupo tiene 3 integrantes.

| Rol | Responsabilidad |
|---|---|
| Coordinación Git | Crea la rama, hace commit, push y abre el PR. |
| Desarrollo | Escribe la modificación acordada. |
| Testing y registro | Prueba la app y completa las respuestas. |

Los tres integrantes revisan el cambio antes del commit y antes del Pull Request.

---

## 5. Tareas por grupo

Cada grupo crea la rama indicada y hace solo la modificación asignada.

Todos los grupos deben agregar sus integrantes en `doc/grupos.md`.

| Grupo | Rama | Archivo principal | Tarea |
|---|---|---|---|
| 1 | `grupo-01-observacion-app` | `README.md` | Agregar una observación sobre de qué se trata la app. |
| 2 | `grupo-02-como-jugar` | `README.md` | Agregar una recomendación breve para jugar por primera vez. |
| 3 | `grupo-03-prueba-juego` | `doc/instructivo.md` | Agregar una recomendación para probar el juego antes de modificar. |
| 4 | `grupo-04-descripcion-simon` | `doc/simon-proa.md` | Mejorar la descripción del juego con una frase clara. |
| 5 | `grupo-05-archivos-principales` | `README.md` | Agregar una aclaración breve sobre algún archivo principal. |
| 6 | `grupo-06-testing` | `doc/instructivo.md` | Agregar una pregunta de testing para revisar la app. |
| 7 | `grupo-07-sonidos` | `doc/simon-proa.md` | Agregar una frase sobre el uso de sonidos en el juego. |
| 8 | `grupo-08-git-colaborativo` | `README.md` | Agregar una frase sobre por qué este repo sirve para practicar Git. |

Ejemplo de cambio en `doc/grupos.md`:

```text
## Grupo 1

- Integrantes: Ana Perez, Juan Gomez, Sol Diaz
- Roles: Ana coordinación Git, Juan desarrollo, Sol testing y registro
```

Ejemplo de cambio en el archivo principal:

```text
- Grupo 1: probamos la app y vimos que el juego consiste en repetir una secuencia de colores.
```

No modificar todavía `index.html`, `styles.css` ni `game.js`.

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

## 7. Hacer la modificación pequeña

Modificar:

1. `doc/grupos.md`, para agregar integrantes y roles del grupo.
2. El archivo principal asignado en la tabla.

Antes de seguir:

- guardar los archivos
- revisar los cambios en VS Code
- verificar que el cambio sea pequeño y claro

---

## 8. Commit y push

Revisar primero los cambios:

```bash
git status
```

Hacer commit:

```bash
git add .
git commit -m "Agrego datos y observación del grupo 1"
```

Subir la rama:

```bash
git push -u origin grupo-01-observacion-app
```

Cambiar el nombre de la rama y el mensaje según el grupo.

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
Qué cambiamos:
Cómo lo revisamos:
```

5. Crear el Pull Request.

Responder:

```text
¿Cuál es el enlace al PR?
¿Desde qué rama sale?
¿Hacia qué rama quiere entrar?
¿Por qué no modificamos main directamente?
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

## Próxima clase

Vamos a recuperar la rama desde otra computadora y sincronizar cambios con GitHub.
