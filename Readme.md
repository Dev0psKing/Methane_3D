# 🧪 Methane Molecule (CH₄) - Interactive 3D Visualization

<div align="center">

![Three.js](https://img.shields.io/badge/Three.js-3D-blue?style=for-the-badge&logo=three.js)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?style=for-the-badge&logo=javascript)
![WebGL](https://img.shields.io/badge/WebGL-ShadowMap-red?style=for-the-badge&logo=webgl)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

### *A stunning, interactive 3D model of the Methane molecule with tetrahedral geometry, dynamic lighting, and immersive controls*

[✨ Live Demo](#) • [📖 Documentation](#) • [🎮 Controls](#-interactive-controls) • [🔧 Setup](#-quick-start)

</div>

---

## 📸 Preview

<div align="center">
  <img src="https://via.placeholder.com/800x450/1a1a2e/ffffff?text=Methane+3D+Model+Preview" alt="Methane Molecule Preview" width="80%">
  <br>
  <em>Carbon (red) • Hydrogen (blue) • Emissive bonds • Real-time shadows • Floating particles</em>
</div>

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔴 **Accurate Molecular Structure** | Tetrahedral geometry with precise bond angles (109.5°) |
| 🎨 **High-Quality Materials** | Metallic/roughness PBR materials with emissive bonds |
| 💡 **Dynamic Lighting System** | Directional key light + rim lights + fill lights + ambient + hemisphere |
| 🌟 **Real-time Shadows** | Soft PCF shadows with 2048px shadow maps |
| 🎬 **Smooth Animations** | Gentle molecular rotation + floating particle effects |
| 🖱️ **Interactive Controls** | Orbit, zoom, and rotate with smooth damping |
| 📝 **Educational Labels** | CSS2D atom labels that always face the camera |
| ✨ **Atmospheric Effects** | Floating particles, glow sprites, fog, and decorative rings |
| 📱 **Responsive Design** | Works on desktop and mobile devices |

## 🎮 Interactive Controls

| Action | Control |
|--------|---------|
| 🖱️ **Rotate View** | Click + Drag |
| 🔍 **Zoom In/Out** | Scroll Wheel |
| 📍 **Auto-Rotate** | Subtle built-in oscillation |
| 🎯 **Reset View** | Refresh page |

## 🧪 Molecular Structure

```
        H
       / \
      C   H
     / \ /
    H   H
```

- **Carbon Atom (Center)**: Red sphere with metallic sheen
- **Hydrogen Atoms (4x)**: Blue spheres at tetrahedral vertices
- **Bonds**: White cylinders with blue emissive glow
- **Bond Length**: 1.75 units (optimized for visual clarity)
- **Geometry**: Perfect tetrahedral arrangement

## 🚀 Quick Start

### Prerequisites
- Modern web browser with WebGL support
- No build tools required! (Pure HTML/CSS/JS)

### Method 1: Direct Download
```bash
git clone https://github.com/yourusername/methane-3d-model.git
cd methane-3d-model
open index.html
```

### Method 2: Live Server (Recommended)
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using VS Code
# Install "Live Server" extension → Right-click index.html → Open with Live Server
```

### Method 3: Deploy to GitHub Pages
1. Push this repository to GitHub
2. Go to Settings → Pages
3. Set source to `main` branch
4. Your site will be live at `https://yourusername.github.io/methane-3d-model`

## 🎨 Visual Highlights

### Lighting Setup
- **Directional Light (Key)** - Casts sharp, realistic shadows
- **Rim Light** - Highlights edges for depth perception
- **Fill Lights** - Eliminates harsh shadows
- **Hemisphere Light** - Simulates environmental bounce
- **Dynamic Intensity** - Subtle pulsating for atmosphere

### Particle Systems
- ✨ **800 ambient particles** - Floating science vibe
- ✨ **400 glow particles** - Energy feel around bonds
- ✨ **12 orbiting spheres** - Extra visual interest

### Ground Plane
- 🌿 Rich green material with slight metalness
- 📏 Grid helper overlay (barely visible, adds reference)
- 🔽 Receives all shadows from the molecule

## 📁 Project Structure

```
methane-3d-model/
├── index.html              # Main application (single file)
├── README.md               # This beautiful documentation
└── assets/                 # (Optional) External resources
    └── screenshots/        # Preview images
```

## 🔧 Technical Details

### Built With
- **[Three.js r160](https://threejs.org/)** - Core 3D rendering engine
- **WebGL** - Hardware-accelerated graphics
- **CSS2DRenderer** - Always-facing text labels
- **OrbitControls** - Smooth camera manipulation

### Performance Optimizations
- ✅ Shadow map size: 2048x2048 (balanced quality/performance)
- ✅ Geometry detail: 32-64 segments (smooth but efficient)
- ✅ Frustum culling enabled
- ✅ RequestAnimationFrame for smooth 60fps
- ✅ Particle count optimized for mobile

### Browser Support
| Chrome | Firefox | Safari | Edge | Mobile |
|--------|---------|--------|------|--------|
| ✅ 90+ | ✅ 88+  | ✅ 14+ | ✅ 90+ | ✅ iOS 15+ |

## 🎯 Educational Value

This visualization is perfect for:
- 🧑‍🔬 **Chemistry students** - Understanding tetrahedral geometry
- 🎓 **Teachers** - Classroom demonstrations
- 💻 **Developers** – Learning Three.js and 3D graphics
- 🎨 **Designers** – Inspiration for scientific visualizations

### Key Concepts Demonstrated
- Tetrahedral molecular geometry (sp³ hybridization)
- Bond angles: 109.5°
- Van der Waals radii visualization
- Shadow casting and receiving in 3D space
- Particle systems for atmosphere

## 🛠️ Customization

Want to tweak the model? Open `index.html` and modify these variables:

```javascript
// Visual adjustments
const bondLength = 1.75;        // Bond distance
const carbonRadius = 0.58;      // Carbon atom size
const hydrogenRadius = 0.42;    // Hydrogen atom size

// Colors (Hex values)
carbonMaterial.color = 0xdd3b3b;    // Red for Carbon
hydrogenMat.color = 0x4d9eff;       // Blue for Hydrogen
planeMaterial.color = 0x2c9a4e;     // Green ground

// Animation speed
moleculeGroup.rotation.y = Math.sin(time * 0.2) * 0.15;  // Adjust multiplier
```

## 📸 Screenshots

<div align="center">
  <table>
    <tr>
      <td><img src="https://via.placeholder.com/300x200/1a1a2e/ffffff?text=Top+View" alt="Top View"></td>
      <td><img src="https://via.placeholder.com/300x200/1a1a2e/ffffff?text=Side+View" alt="Side View"></td>
    </tr>
    <tr>
      <td><img src="https://via.placeholder.com/300x200/1a1a2e/ffffff?text=Shadow+Details" alt="Shadows"></td>
      <td><img src="https://via.placeholder.com/300x200/1a1a2e/ffffff?text=Atmosphere" alt="Particles"></td>
    </tr>
  </table>
</div>

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 **Fork** the repository
2. 🔧 **Create** a feature branch (`git checkout -b feature/amazing`)
3. 💾 **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. 📤 **Push** to the branch (`git push origin feature/amazing`)
5. ✅ **Open** a Pull Request

### Ideas for Improvements
- [ ] Add bond angle measurements display
- [ ] Implement VR mode (WebXR)
- [ ] Add different molecular representations (ball-and-stick vs space-filling)
- [ ] Include electron cloud visualization
- [ ] Add audio descriptions for accessibility

## 📄 License

Distributed under the **MIT License**. See `LICENSE` file for more information.

```
MIT License

Copyright (c) 2024 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files...
```

## 🙏 Acknowledgments

- **Three.js Team** – For the incredible 3D library
- **Chemistry Educators** – For inspiring molecular visualizations
- **Open Source Community** – For tools and resources

## 📬 Contact

**Your Name** - [@Dev0psKing](https://twitter.com/Dev0psKing) - uwabor@zohomail.com

---

<div align="center">
  
### ⭐ Star this repo if you found it useful! ⭐

**Made with ❤️ and Three.js**


</div>