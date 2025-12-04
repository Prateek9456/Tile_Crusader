# 🗡️ TILE CRUSADER

A fast-paced, roguelike dungeon crawler built with HTML5 and JavaScript. Pick up a random crusade and dive into procedurally generated dungeons in just minutes!

![Game Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange)

## 📖 About

Tile Crusader is a crowd-sourced, coffee break, roguelike game designed for quick play sessions. Perfect for playing between tasks at work, while waiting for water to boil, or during downtime. With simplified gameplay and no long-term character building, each crusade offers a fresh, fast RPG experience!

## ✨ Features

- **Three Unique Character Classes**
  - 🛡️ Knight: High health and balanced combat
  - 🔮 Mage: Magic-focused with strong defense
  - 🗡️ Thief: Agile with large inventory space

- **Dynamic Combat System**
  - Range-based attack and defense values
  - Strategic equipment choices
  - Real-time damage calculation

- **Procedural Generation**
  - Random dungeon layouts every playthrough
  - 9 different monster types
  - Hidden treasures and traps

- **Equipment & Progression**
  - 18+ items to collect (weapons, armor, shields, helmets)
  - Level up system between crusades
  - Choose stat upgrades after each level

- **Roguelike Elements**
  - Permadeath per level (restart on death)
  - Fog of war exploration
  - Random loot drops

## 🎮 How to Play

### Starting the Game
1. Choose your character class (Knight, Mage, or Thief)
2. Each class has different starting stats and inventory space
3. Navigate through the dungeon to find the exit

### Controls
| Key | Action |
|-----|--------|
| **Arrow Keys** | Move player |
| **Walk into enemies** | Initiate combat |
| **Walk into chests** | Open chest |
| **P** | Use potion (heals 50% of max HP) |
| **ESC** | Return to menu |

### Combat
- Walk into an enemy to attack automatically
- Damage is calculated: `Attack - Enemy Defense = Damage Dealt`
- Both attack and defense have random variance (±2)
- Enemies counter-attack each turn
- Defeat enemies to gain kill points and possible loot

### Exploration
- Tiles are revealed as you explore (4-tile vision range)
- **Chests** contain:
  - Gold (30% chance)
  - Potions (20% chance)
  - Equipment (10% chance)
  - Traps (20% chance - deals 2 damage)
  - Nothing (30% chance)

### Winning & Progression
- Reach the green EXIT tile to complete the level
- Choose a stat upgrade between levels:
  - Max Life (+2)
  - Attack (+1)
  - Defense (+1)
  - Potions (+2)
  - Inventory Space (+2)
- Continue through increasingly challenging crusades

### Death
- If HP reaches 0, you restart the current level
- Death counter tracks total deaths
- All inventory and equipped items are lost
- Kill count and level persist across deaths

## 🚀 Installation & Setup

### Option 1: Direct Browser (Easiest)
```bash
1. Download the tile-crusader.html file
2. Double-click to open in your default browser
3. Start playing immediately!
```

### Option 2: Local Web Server (Recommended)

**Using Python:**
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Open browser to: http://localhost:8000/tile-crusader.html
```

**Using Node.js (http-server):**
```bash
# Install http-server globally
npm install -g http-server

# Run in the game directory
http-server -p 8000

# Open browser to: http://localhost:8000/tile-crusader.html
```

**Using PHP:**
```bash
php -S localhost:8000

# Open browser to: http://localhost:8000/tile-crusader.html
```

### Option 3: VS Code Live Server
1. Install the "Live Server" extension in VS Code
2. Right-click `tile-crusader.html`
3. Select "Open with Live Server"
4. Game opens automatically in your browser

## 📊 Game Statistics

### Character Classes

| Class | Max Life | Attack | Defense | Potions | Inventory |
|-------|----------|--------|---------|---------|-----------|
| Knight | 9 | 3 | 2 | 4 | 4 slots |
| Mage | 5 | 2 | 4 | 5 | 4 slots |
| Thief | 7 | 2 | 1 | 2 | 8 slots |

### Monster Types
- **Ork** - Balanced fighter
- **Ogre** - Heavy hitter
- **Goblin** - Weak but numerous
- **Wolfman** - Fast attacker
- **Vampire** - Life drainer
- **Mummy** - High defense
- **Skeleton** - Undead warrior
- **Imp** - Demon spawn
- **Gargoyle** - Stone defender

### Equipment

**Weapons** (Increases Attack):
- Club (+1) → Dagger (+2) → Mace (+3) → Hammer (+4) → Axe (+5) → Sword (+6)

**Shields** (Increases Defense):
- Round Shield (+2) → Warrior Shield (+3) → Oval Shield (+5) → Long Shield (+7)

**Helmets** (Increases Defense):
- Bucket Helmet (+2) → Roman Helmet (+3) → Full Helmet (+5) → Fuller Helmet (+7)

**Armor** (Increases Defense):
- Light Chainmail (+1) → Chainmail (+2) → Chest Armor (+5) → Full Armor (+7)

## 🎯 Game Tips & Strategy

1. **Equipment Matters**: Always equip the best gear you find
2. **Potion Management**: Save potions for tough fights or boss encounters
3. **Exploration**: Check all chests, but be ready for traps
4. **Class Strategy**:
   - Knight: Tank through battles with high HP
   - Mage: Use high defense to minimize damage
   - Thief: Carry more potions and equipment for versatility
5. **Upgrade Wisely**: Balance offense and defense based on your playstyle
6. **Know When to Flee**: You can exit levels without killing all monsters

## 🛠️ Technical Details

- **Technology Stack**: HTML5 Canvas, Vanilla JavaScript, CSS3
- **Canvas Size**: 800x600 pixels
- **Tile Size**: 32x32 pixels
- **Map Size**: 25x19 tiles
- **No External Dependencies**: Runs completely offline

## 📁 Project Structure

```
tile-crusader/
│
├── tile-crusader.html          # Main game file (all-in-one)
├── README.md                   # This file
└── LICENSE                     # MIT License
```

## 🐛 Known Issues & Limitations

- Inventory system is visual but item management could be enhanced
- No sound effects or music (planned for future versions)
- Monster AI is static (they don't move)
- No save/load system between browser sessions
- Equipment equipping is automatic, no manual selection UI yet

## 🔮 Future Enhancements

- [ ] Boss battles with unique mechanics
- [ ] Sound effects and background music
- [ ] More complex dungeon generation (rooms, corridors)
- [ ] Special abilities per character class
- [ ] Achievements and unlockables
- [ ] Local storage for saving progress
- [ ] Mobile touch controls
- [ ] Multiplayer mode
- [ ] More monster varieties
- [ ] Status effects (poison, stun, etc.)

## 🤝 Contributing

This is a sample project based on a Game Design Document. Feel free to fork and modify for your own purposes!

### How to Contribute:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2024 Tile Crusader

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 📞 Support

Having issues? Here are some common solutions:

**Game won't load?**
- Ensure JavaScript is enabled in your browser
- Try a different browser (Chrome, Firefox, Safari, Edge)
- Check browser console for errors (F12)

**Controls not working?**
- Click on the game canvas to focus it
- Ensure you're not in a text input field
- Try refreshing the page

**Performance issues?**
- Close other browser tabs
- Update your browser to the latest version
- Reduce browser zoom level

## 🎓 Learning Resources

This game was created as an educational project. Developers can learn:
- HTML5 Canvas rendering
- Game loop implementation
- Procedural generation algorithms
- Combat system design
- State management in vanilla JavaScript

## 👏 Credits

- **Original Concept**: Based on the Tile Crusader GDD
- **Development**: Built with ❤️ using HTML5 and JavaScript
- **Inspiration**: Classic roguelike games and dungeon crawlers

---

**Ready to crusade?** Load up the game and start your adventure! ⚔️

*Remember: Each crusade is unique. No two dungeons are the same!*
