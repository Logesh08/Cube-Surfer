# Cube Surfer - 3D Endless Runner Game

## Overview
Cube Surfer is an exciting endless runner game built with Three.js where you control a yellow cube avoiding obstacles while being chased by a mysterious red cube. The game features dynamic lane-switching mechanics, collision detection, and increasing difficulty as you progress.

## Features
- Endless running gameplay with increasing difficulty
- Three-lane movement system with smooth transitions
- Dynamic obstacle generation (trains)
- Mysterious red cube chase mechanics
- Real-time score tracking
- Advanced collision detection
- Responsive design for all screen sizes
- Dynamic shadow and lighting effects

## Game Mechanics
- Use **Left Arrow** and **Right Arrow** keys to switch lanes
- Avoid hitting trains head-on
- Watch out for the red cube chasing you
- Score increases as you survive longer
- Game ends on collision with obstacles

## Prerequisites
- Modern web browser with WebGL support
- Basic understanding of HTML and JavaScript
- Local development server (optional)

## Installation & Setup

1. Clone the repository:

```bash
git clone https://github.com/yourusername/cube-surfer.git
cd cube-surfer
```

2. Start a local server:
   - Using Python 3:
   ```bash
   python -m http.server
   ```
   - Using Node.js:
   ```bash
   npx http-server
   ```

3. Open your browser and navigate to:
   - `http://localhost:8000` (Python)
   - `http://localhost:8080` (Node.js)

## Technical Details
- Built with Three.js for 3D rendering
- Uses WebGL for hardware acceleration
- Implements requestAnimationFrame for smooth animations
- Features dynamic obstacle spawning system
- Includes advanced collision detection using Three.js Box3

## Performance Optimization
- Efficient obstacle pooling system
- Optimized track segment recycling
- Minimal DOM updates for score display
- Hardware-accelerated animations

## Browser Compatibility
- Chrome (recommended)
- Firefox
- Safari
- Edge
- Any modern browser with WebGL support

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Three.js team for the amazing 3D library
- Inspiration from classic endless runner games
- Community feedback and contributions

