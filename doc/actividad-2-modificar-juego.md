# Actividad 2: modificar el juego y ver el resultado publicado

## Objetivo

Hacer un Pull Request que modifique una parte pequeña del juego Simon.

En esta actividad sí vamos a tocar archivos de la app:

```text
index.html
styles.css
game.js
```

Después de que el docente revise y haga merge a `main`, vamos a observar el producto final publicado en Vercel:

```text
https://simon-proa-2026.vercel.app/
```

---

## 1. Antes de empezar

Cada grupo puede estar en una situación distinta.

Si todavía no clonaron el repositorio:

```bash
git clone https://github.com/lole-s/simon-proa-2026.git
cd simon-proa-2026
```

Si ya lo habían clonado:

```bash
git status
git switch main
git pull origin main
```

Si tienen cambios sin commit, avisen antes de hacer `pull`.

Regla para esta actividad:

```text
Cada actividad usa una rama nueva.
No trabajar sobre la rama de la actividad anterior.
```

---

## 2. Probar la versión publicada

Abrir:

```text
https://simon-proa-2026.vercel.app/
```

Responder:

```text
¿Qué se ve al abrir la app publicada?
¿Qué textos aparecen?
¿Cómo se inicia el juego?
¿Qué cambio le haría tu grupo para mejorarla?
```

---

## 3. Crear una rama nueva

Cada grupo usa la rama indicada en la tabla.

Ejemplo:

```bash
git switch -c act2-G1-textos
```

Verificar:

```bash
git branch
```

---

## 4. Tareas por grupo

Cada grupo hace solo la tarea asignada.

| Grupo | Rama | Archivos | Tarea |
|---|---|---|---|
| 1 | `act2-G1-textos` | `index.html`, `game.js` | Cambiar textos iniciales al español. |
| 2 | `act2-G2-instrucciones` | `index.html`, `styles.css` | Agregar instrucciones breves para jugar. |
| 3 | `act2-G3-creditos` | `index.html`, `styles.css` | Agregar créditos del curso. |
| 4 | `act2-G4-colores` | `styles.css` | Cambiar colores de fondo, textos o botones. |
| 5 | `act2-G5-efecto-botones` | `styles.css` | Agregar sombra o efecto visual al presionar botones. |
| 6 | `act2-G6-nivel-titulo` | `game.js` | Mostrar el nivel actual en el título de la pestaña. |
| 7 | `act2-G7-bienvenida` | `index.html`, `game.js` | Mostrar un mensaje de bienvenida al iniciar. |
| 8 | `act2-G8-botones-2x2` | `styles.css` | Mejorar forma, bordes o distribución 2x2 de los botones. |

Antes de modificar, el grupo debe decidir:

```text
¿Qué archivo vamos a tocar?
¿Qué parte exacta del juego cambia?
¿Cómo vamos a probar que sigue funcionando?
```

---

## 5. Probar localmente

Abrir `index.html` en el navegador y probar:

- la página carga
- el juego inicia
- los botones responden
- el cambio del grupo se ve o funciona
- no se rompió una parte que antes funcionaba

Responder:

```text
¿Qué cambio hizo el grupo?
¿Cómo lo probaron?
¿Qué podría revisar otro grupo en el PR?
```

---

## 6. Commit y push

Revisar cambios:

```bash
git status
```

Hacer commit:

```bash
git add .
git commit -m "Mejoro textos iniciales del juego"
```

Subir la rama:

```bash
git push -u origin act2-G1-textos
```

Cambiar el mensaje y la rama según el grupo.

---

## 7. Crear Pull Request

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
Cómo lo probamos:
Qué debería revisar el docente:
```

5. Crear el Pull Request.

---

## 8. Después del merge

El docente revisa y hace merge a `main`.

Después del merge, Vercel actualiza la app publicada.

Volver a abrir:

```text
https://simon-proa-2026.vercel.app/
```

Responder:

```text
¿El cambio de tu grupo aparece en la app publicada?
¿Qué otros cambios aparecen?
¿Qué pasó entre el merge en GitHub y la actualización en Vercel?
```

---

## Entrega

```text
Grupo:
Integrantes:
Rama:
Archivos modificados:
Cambio realizado:
Cómo lo probaron:
Enlace al PR:
¿Se ve en Vercel después del merge?
```
