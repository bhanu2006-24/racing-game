# 🏎️ Poly City Racer: Turbo

A high-octane 3D racing game built with **Three.js** featuring neon-lit cyberpunk cityscapes, intense AI competition, and adrenaline-pumping nitro boosts!

![Racing Game](https://img.shields.io/badge/Game-Racing-ff3366?style=for-the-badge)
![Three.js](https://img.shields.io/badge/Three.js-r128-00ffcc?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## 🎮 Features

### 🌃 **Immersive 3D Environment**
- Procedurally generated cyberpunk city with **350+ buildings**
- Dynamic neon-lit skyscrapers with emissive lighting
- Smooth curved racing track through the urban landscape
- Atmospheric fog and professional lighting system

### 🏁 **Competitive Racing**
- Race against **3 AI opponents** with unique personalities
- **3-lap race** system with real-time position tracking
- Smart AI that navigates the track and avoids collisions
- Dynamic difficulty - AI competitors trade positions naturally

### 🚗 **Advanced Car Physics**
- Realistic acceleration, friction, and turning mechanics
- **Nitrous boost system** - Hold `SHIFT` for speed bursts
- Drift mechanics with visual particle effects
- Building collision detection and response
- Dynamic camera with speed-based FOV adjustments

### 🎨 **Premium Visual Effects**
- Real-time minimap with all racer positions
- Particle system for drift and nitro trails
- Dynamic spotlights from car headlights
- Smooth shadows and reflections
- Cyberpunk color palette (pink, cyan, yellow, purple)

### 📊 **Race HUD**
- Live speedometer (KM/H)
- Position tracker (1st/2nd/3rd/4th with color coding)
- Lap counter
- Nitrous fuel gauge with visual bar
- Circular minimap showing track and all racers

## 🎯 How to Play

### Controls
| Key | Action |
|-----|--------|
| `W` / `↑` | Accelerate |
| `S` / `↓` | Brake/Reverse |
| `A` / `←` | Turn Left |
| `D` / `→` | Turn Right |
| `SHIFT` | Nitrous Boost |
| `SPACE` | Brake |
| `R` | Reset Car Position |

### Gameplay Tips
1. **Start Strong**: Get ahead in the first lap to maintain your lead
2. **Drift Corners**: Use controlled drifting to maintain speed through turns
3. **Nitro Strategy**: Save nitrous for straightaways to maximize speed
4. **Avoid Buildings**: Collisions will reverse your momentum - stay on track!
5. **Watch the Minimap**: Keep an eye on opponent positions

## 🚀 Getting Started

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/racing-game.git
   cd racing-game
   ```

2. **Open the game**
   ```bash
   # Simply open index.html in your browser
   open index.html
   # or
   # Right-click index.html → Open with → Your Browser
   ```

### Running a Local Server (Optional)

For the best experience, run with a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if you have http-server installed)
npx http-server -p 8000
```

Then visit `http://localhost:8000` in your browser.

## 🛠️ Technical Details

### Built With
- **Three.js** (r128) - 3D graphics library
- **Vanilla JavaScript** (ES6+) - Game logic
- **HTML5** - Structure
- **CSS3** - UI styling

### Architecture

```
racing-game/
│
├── index.html          # Main game file (self-contained)
├── README.md          # Documentation
├── LICENSE            # MIT License
└── .gitignore         # Git ignore rules
```

### Key Components

**Game Engine**
- `CarController` class - Handles physics, AI, and player input
- `ParticleSystem` class - Visual effects for drifting and nitro
- Track generation using Catmull-Rom curves
- Procedural city generation with collision detection

**Physics System**
- Velocity-based movement
- Friction simulation
- Turn speed mechanics
- Collision detection and response
- Lap progress calculation using track projection

**AI System**
- Pathfinding along track curve
- Look-ahead targeting
- Speed variation for realistic racing
- Collision avoidance

## 🎨 Customization

### Modify Car Colors
Edit the `COLORS` array in `index.html`:
```javascript
const COLORS = [0xff3366, 0x00ccff, 0xccff00, 0xcc00ff];
// Player, AI1, AI2, AI3
```

### Adjust Track Size
Change the `TRACK_SCALE` constant:
```javascript
const TRACK_SCALE = 1.2; // Default: 1.2
```

### Modify Physics
Adjust car properties in `CarController`:
```javascript
this.acceleration = 0.035;  // Acceleration rate
this.maxSpeed = 2.4;        // Max speed
this.turnSpeed = 0.045;     // Turn rate
this.nitroMaxSpeed = 3.5;   // Nitro max speed
```

### Change Number of Laps
```javascript
const TOTAL_LAPS = 3; // Default: 3
```

## 🐛 Known Issues & Future Improvements

### Current Limitations
- Single track layout (can be expanded)
- No sound effects (music/SFX to be added)
- No power-ups or collectibles
- No multiplayer support

### Planned Features
- 🎵 Sound effects and background music
- 🏆 Multiple tracks and difficulty levels
- ⚡ Power-ups and boost pads
- 💾 Save/load race times and records
- 🎯 Time trial mode
- 📱 Mobile touch controls
- 🌐 Multiplayer racing

## 📸 Screenshots

**Coming Soon!** - Capture your best racing moments and share them!

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Bhanu Pratap Saini**
- GitHub: [@bhanu2006-24](https://github.com/bhanu2006-24)

## 🙏 Acknowledgments

- **Three.js** team for the amazing 3D library
- Inspiration from classic arcade racing games
- Cyberpunk aesthetic and neon city vibes

## 🌟 Show Your Support

Give a ⭐️ if you enjoyed playing this game!

---

**Ready to race?** Fire up your engine and dominate the neon streets! 🏁💨
