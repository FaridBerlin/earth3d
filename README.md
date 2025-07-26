# 🌍 Earth 3D Visualization

A stunning interactive 3D Earth visualization built with Three.js, featuring realistic textures, atmospheric effects, and smooth animations.

![Earth 3D Preview](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![WebGL](https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white)

## 🚀 Live Demo

**[🌍 View Live Demo](https://faridberlin.github.io/earth3d/)**

## ✨ Features

- 🌍 **Realistic Earth Textures** - High-quality Earth surface mapping
- ☁️ **Dynamic Cloud Layers** - Animated cloud formations with transparency
- 🌃 **City Lights Effect** - Glowing city lights on the night side
- 🌟 **Atmospheric Glow** - Fresnel-based atmospheric scattering effect
- ⭐ **Rotating Starfield** - Beautiful background star field
- 🎮 **Interactive Controls** - Mouse/touch orbit controls for exploration
- 📱 **Responsive Design** - Adapts to all screen sizes
- ⚡ **Smooth Animations** - 60fps performance with optimized rendering

## 🎥 Preview

```
    🌍 Interactive Earth Visualization
    ├── Realistic surface textures
    ├── Animated cloud layers
    ├── Glowing atmospheric effects
    ├── City lights at night
    └── Immersive starfield background
```

## 🛠️ Technologies Used

- **[Three.js](https://threejs.org/)** - 3D graphics library
- **WebGL** - Hardware-accelerated 3D rendering
- **JavaScript ES6+** - Modern JavaScript features
- **HTML5 Canvas** - Rendering surface
- **Import Maps** - Module resolution

## 🏗️ Project Structure

```
earth3d/
├── index.html              # Main HTML file
├── index.js                # Main JavaScript application
├── src/
│   ├── getStarfield.js     # Starfield generation
│   └── getFresnelMat.js    # Atmospheric glow shader
├── textures/
│   ├── 00_earthmap1k.jpg   # Earth surface texture
│   ├── 01_earthbump1k.jpg  # Earth bump/height map
│   ├── 02_earthspec1k.jpg  # Earth specular map
│   ├── 03_earthlights1k.jpg # City lights texture
│   ├── 04_earthcloudmap.jpg # Cloud layer texture
│   ├── 05_earthcloudmaptrans.jpg # Cloud transparency
│   └── stars/
│       └── circle.png      # Star particle texture
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Modern web browser with WebGL support
- Local development server (for local testing)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/FaridBerlin/earth3d.git
   cd earth3d
   ```

2. **Serve locally** (choose one method)
   
   **Option A: Python**
   ```bash
   python -m http.server 8000
   ```
   
   **Option B: Node.js**
   ```bash
   npx serve .
   ```
   
   **Option C: Live Server (VS Code)**
   - Install Live Server extension
   - Right-click `index.html` → "Open with Live Server"

3. **Open in browser**
   ```
   http://localhost:8000
   ```

## 🎮 Controls

- **Mouse Drag** - Rotate the Earth
- **Mouse Wheel** - Zoom in/out
- **Touch Drag** - Rotate on mobile devices
- **Pinch** - Zoom on mobile devices

## 🎨 Customization

### Modify Animation Speed
```javascript
// In index.js, adjust rotation speeds
earthMesh.rotation.y += 0.009;    // Earth rotation
cloudsMesh.rotation.y += 0.0093;  // Cloud rotation (slightly faster)
stars.rotation.y -= 0.0009;       // Star field rotation
```

### Change Earth Tilt
```javascript
// Adjust Earth's axial tilt (currently 23.4°)
earthGroup.rotation.z = -23.4 * Math.PI / 180;
```

### Customize Lighting
```javascript
// Modify sun light properties
const sunLight = new THREE.DirectionalLight(0xffffff, 2.0);
sunLight.position.set(-2, 0.5, 1.5);
```

## 🌟 Key Features Explained

### Realistic Earth Rendering
- **Surface Mapping**: High-resolution Earth texture
- **Bump Mapping**: Adds surface detail and depth
- **Specular Mapping**: Controls surface reflectivity for realistic oceans

### Atmospheric Effects
- **Fresnel Glow**: Custom shader for atmospheric scattering
- **Cloud Layers**: Semi-transparent animated clouds
- **City Lights**: Additive blending for nighttime illumination

### Performance Optimizations
- **Icosphere Geometry**: Efficient sphere representation
- **Texture Loading**: Optimized texture management
- **Efficient Rendering**: 60fps with proper frame timing

## 🤝 Contributing

Contributions are welcome! Here are some ideas:

- 🎨 **Visual Enhancements**
  - Add moon and sun objects
  - Implement day/night cycle
  - Add aurora effects
  
- 🚀 **Features**
  - Satellite tracking
  - Weather data integration
  - Real-time lighting based on location
  
- 🐛 **Bug Fixes**
  - Mobile performance improvements
  - Browser compatibility fixes

### Development Setup

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📚 Learning Resources

- **Original Tutorial**: [YouTube Tutorial](https://youtu.be/FntV9iEJ0tU)
- **Earth Textures**: [PlanetPixelEmporium](https://planetpixelemporium.com/earth.html)
- **Three.js Documentation**: [threejs.org](https://threejs.org/docs/)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **Three.js Community** - For the amazing 3D library
- **NASA** - For Earth texture references
- **WebGL Community** - For graphics programming resources
- **PlanetPixelEmporium** - For high-quality Earth texture maps

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/FaridBerlin/earth3d?style=social)
![GitHub forks](https://img.shields.io/github/forks/FaridBerlin/earth3d?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/FaridBerlin/earth3d?style=social)

---

**Made with ❤️ by [Farid Berlin](https://github.com/FaridBerlin)**

*If you found this project helpful, please consider giving it a ⭐!*