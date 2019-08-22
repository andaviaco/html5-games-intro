---
marp: true
title: Videojuegos con HTML5
theme: gaia
paginate: true
_paginate: false
---

<!-- _class: gaia lead -->

# <!--fit--> Videojuegos con HTML5

Andrés Ávila Acosta
[@andaviaco](https://github.com/andaviaco)

---
# 💁‍♂️ Yo

- Lead Software Engineer
- Developer Circles Guadalajara
- Estudiante de Ing. Computación
- 4+ años como desarrollador

---
# ¿Qué es HTML5?
![bg left: 50% ](img/html5-logo.png)
![bg left: 90%](img/html5-areas.png)

---
<!-- _class: invert -->
![bg 100%](img/2d-demo.gif)


---
<style scoped>
h1 {
  text-align: center;
}
</style>
<!-- _class: invert -->
![bg 100%](img/3d-demo.gif)

---
![bg](#123)
<!-- _class: invert -->
## HTML5: Ventajas 👍
* Juegos multiplataforma

* Desarrollo en plataformas móviles nativas

* Fácil distribución

* Compatibles con nuevas plataformas como Facebook Instant Games

---
## HTML5: Desventajas 👎
* Menor rendimiento que una plataforma nativa

* Calidad de los gráficos


---
##  Instant Games
![bg 70%](img/instant-games.png)


---
<!-- _class: lead -->
# <!-- fit --> ¿Qué necesito aprender?

---
![bg 70%](img/html-css-js.webp)

---
<style scoped>
h3 {
  text-align: center;
}
</style>

### Diseño y modelado
![bg left: 80%](img/blender-logo.png)
![bg right: 80%](img/illustrator.png)

---
<!-- _class: lead -->
# <!-- fit --> ¿Cómo se hace un videojuego con HTML5?

---
## Elemento canvas
```html
<!-- index.html -->

<!doctype html>
<html>
  <head>
    <title>My Awesome Game</title>
  </head>
  <body>
    <canvas id="main-canvas" width="600" height="800"></canvas>
    <script src="main.js"></script>
  </body>
</html>
```

---
## Dibujo 2D
```js
// main.js

const assets = require('./assets.js');

const canvas = document.getElementById('main-canvas');
const context = canvas.getContext('2d');

assets.loadImage('images/green_blob.png').then(img => {
    context.drawImage(img, 25, 25);
});
```

---
## Animación
```javascript
// main.js

function drawGame() {
  entities.forEach(entity => {
    entity.draw(gameCanvas);
  });
  requestAnimationFrame(drawGame);
}
```

---
## Almacenamiento de datos
#### Local Storage
- Almacenar información del usuario en el dispositivo
- Es eliminado al limpiar el caché
```js
// Alamcenar progreso del jugador

localStorage.setItem('game_state', JSON.stringify(gameState));
```

---
# Frameworks y herramientas
<!-- _class: lead  -->

---
<style scoped>
h3 {
  text-align: center;
}
</style>
### 2D
![bg left: 50%](img/pixijs.png)
![bg right: 50%](img/canvas.png)

---
### 3D
<style scoped>
h3 {
  text-align: center;
}
</style>
![bg left: 50%](img/threejs-1.png)
![bg right: 50%](img/webGL.svg)

---

### Audio
<style scoped>
h3 {
  text-align: center;
}
</style>
![bg 70%](img/howlerjs.svg)

---
<style scoped>
h3 {
  text-align: center;
}
</style>

### Motores
![bg left: 100%](img/babylonjs.png)
![bg left: 50%](img/phaser.png)
![bg left: 50%](img/unity.png)

---
### Editores (Game Maker)
<style scoped>
h3 {
  text-align: center;
}
</style>
![bg left: 50%](img/construct.png)
![bg right: 50%](img/gdevelop.png)

---
# Eligiendo la mejor herramienta
* ¿Qué tipo de juego quiero?
* ¿Dónde lo quiero jugar?
* ¿Qué tipo de graficos quiero que tenga?


---
# El "Dream Team"
Conocimiento multidiciplinario.
- Diseño gráfico y animación
- Audio
- Desarrollo
- Matemáticas y física
- Marketing

---
# Recursos
HTML5 Game Engines
https://html5gameengine.com

Matemáticas esenciales para programadores de videojugos
http://www.essentialmath.com/book.htm

---
# Más recursos gratuitos
Música, efectos de sonido y texturas libres de derechos
https://soundimage.org

Gráficos grátis
http://hasgraphics.com/

Arte para videojuegos
https://opengameart.org/

Blog enfocado en la industria de los videojuegos
http://www.lostgarden.com

---
<!-- _class: lead -->
# ¿Preguntas?


---
<!-- _class: lead -->
# ¡Gracias!
[@andaviaco](https://github.com/andaviaco)
