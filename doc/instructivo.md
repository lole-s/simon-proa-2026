# Instructivo Simon Proa 2026

## Objetivo

Trabajar en grupos sobre el mismo repositorio usando este flujo:

```text
clonar -> crear rama -> modificar -> commit -> push -> Pull Request -> merge -> pull
```

Repositorio:

```text
https://github.com/lole-s/simon-proa-2026
```

---

## Requisitos

- Tener Git instalado.
- Tener Visual Studio Code instalado.
- Tener cuenta de GitHub.
- Haber aceptado la invitacion al repositorio.
- Haber iniciado sesion en GitHub desde VS Code.

---

## Grupos de trabajo

Cada grupo tiene 3 integrantes.

Roles:

| Rol | Responsabilidad |
|---|---|
| Coordinacion Git | Crea la rama, revisa commits y publica la rama |
| Desarrollo | Modifica los archivos de la tarea |
| Testing | Prueba que el juego siga funcionando |

Los tres integrantes revisan el cambio antes de crear el Pull Request.

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

Desde terminal:

```bash
cd /c/temp2026/Testing2026_APELLIDO/Eje_1_Software_Colaborativo
git clone https://github.com/lole-s/simon-proa-2026.git
cd simon-proa-2026
code .
```

---

## 2. Probar antes de modificar

Abrir:

```text
index.html
```

Probar:

- carga la pagina
- funcionan los botones
- no hay errores visibles
- el juego se puede iniciar

---

## 3. Actualizar `main`

Antes de crear una rama:

```bash
git switch main
git pull origin main
```

---

## 4. Crear rama de trabajo

Cada grupo crea la rama indicada en la tabla.

Ejemplo:

```bash
git switch -c tarea-01-creditos-curso
```

Verificar:

```bash
git branch
```

---

## 5. Tareas por grupo

| Grupo | Rama | Archivos | Tarea |
|---|---|---|---|
| 1 | `tarea-01-creditos-curso` | `index.html`, `styles.css` | Agregar una seccion `Creditos del curso` que represente a todo el curso. Incluir curso, anio, escuela y una frase grupal. |
| 2 | `tarea-02-instrucciones-juego` | `index.html`, `styles.css` | Agregar una seccion `Como jugar` con 3 pasos: mirar la secuencia, repetirla, avanzar de nivel. |
| 3 | `tarea-03-panel-estado` | `index.html`, `styles.css` | Ordenar el panel de estado para que nivel, mensaje y boton de inicio se vean claros. |
| 4 | `tarea-04-estilos-botones` | `styles.css` | Mejorar los cuatro botones: mismo tamanio, bordes consistentes, separacion pareja y efecto hover. |
| 5 | `tarea-05-animacion-activo` | `styles.css`, `game.js` | Mejorar el efecto visual cuando un boton se activa en la secuencia. |
| 6 | `tarea-06-mensaje-bienvenida` | `index.html`, `game.js` | Mostrar un mensaje inicial de bienvenida y cambiarlo al iniciar el juego. |
| 7 | `tarea-07-nivel-visible` | `index.html`, `game.js`, `styles.css` | Hacer que el nivel actual se vea claramente y se actualice al avanzar. |
| 8 | `tarea-08-game-over` | `index.html`, `game.js`, `styles.css` | Mejorar el mensaje de fin de juego e indicar como volver a empezar. |

Cada grupo anota:

```text
Grupo:
Integrantes:
Rama:
Archivos modificados:
Cambio realizado:
Como lo probaron:
```

---

## 6. Hacer commit

Despues de modificar:

1. Guardar archivos.
2. Probar el juego.
3. Revisar cambios en VS Code.
4. Preparar cambios.
5. Hacer commit.

Ejemplos:

```text
Agrego creditos del curso
Mejoro instrucciones del juego
Actualizo estilos de botones
Muestro nivel actual
```

Desde terminal:

```bash
git status
git add .
git commit -m "Agrego creditos del curso"
```

---

## 7. Hacer push

Desde VS Code:

```text
Publish Branch
```

o:

```text
Push
```

Desde terminal:

```bash
git push -u origin tarea-01-creditos-curso
```

---

## 8. Crear Pull Request

En GitHub:

1. Entrar al repositorio.
2. Buscar la rama publicada.
3. Hacer clic en **Compare & pull request**.
4. Escribir titulo claro.
5. Completar:

```text
Grupo:
Integrantes:
Rama:
Que cambiamos:
Como lo probamos:
Archivos modificados:
```

6. Crear el Pull Request.

---

## 9. Revision y merge

El docente revisa cada Pull Request.

El merge lo hace el docente para cuidar la version principal del proyecto.

Si hay conflictos, se resuelven antes del merge.

---

## 10. Traer la version final

Despues de que el docente mergea los Pull Requests, todos actualizan su copia:

```bash
git switch main
git pull origin main
```

Verificar:

```bash
git log --oneline --graph --all
```

---

## Conflictos

Un conflicto aparece cuando dos ramas modifican la misma parte de un archivo.

Si aparece:

1. No cerrar VS Code.
2. Buscar las marcas:

```text
<<<<<<<
=======
>>>>>>>
```

3. Decidir que parte queda.
4. Borrar las marcas.
5. Guardar.
6. Hacer commit de la resolucion.
