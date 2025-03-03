# Simple 3D Game with Three.js

## Overview
This project is a simple 3D game built using Three.js, a popular JavaScript library for creating 3D graphics in the browser.

## Prerequisites
- Basic knowledge of HTML, CSS, and JavaScript
- A code editor (e.g., Visual Studio Code)
- A web browser (e.g., Chrome, Firefox)

## Getting Started

### 1. Set Up Your Project
Create a new directory for your project and navigate into it:

```bash
mkdir simple-3d-game
cd simple-3d-game
```

### 2. Create HTML File
Create an `index.html` file in your project directory:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple 3D Game</title>
    <style>
        body { margin: 0; }
        canvas { display: block; }
    </style>
</head>
<body>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <script src="app.js"></script>
</body>
</html>
```

### 3. Create JavaScript File
Create an `app.js` file in your project directory. This file will contain the main logic for your game.

```javascript
// app.js
import * as THREE from 'three';

// Set up the scene, camera, and renderer
const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
const renderer = new THREE.WebGLRenderer();
renderer.setSize(window.innerWidth, window.innerHeight);
document.body.appendChild(renderer.domElement);

// Add a simple cube
const geometry = new THREE.BoxGeometry();
const material = new THREE.MeshBasicMaterial({ color: 0x00ff00 });
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);

// Set camera position
camera.position.z = 5;

// Animation loop
function animate() {
    requestAnimationFrame(animate);
    cube.rotation.x += 0.01;
    cube.rotation.y += 0.01;
    renderer.render(scene, camera);
}
animate();
```

### 4. Run Your Game
You can use a simple HTTP server to run your game. If you have Python installed, you can run:

```bash
# For Python 3.x
python -m http.server
```

Then, open your browser and navigate to `http://localhost:8000`.

## Next Steps
- Explore Three.js documentation to learn more about adding lights, textures, and more complex geometries.
- Consider adding user controls to interact with the 3D scene.
- Experiment with different shapes and animations to enhance your game.

## License
This project is licensed under the MIT License.
