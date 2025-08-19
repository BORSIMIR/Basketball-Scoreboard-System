# Basketball Scoreboard System 🏀

**[🔗 Live Demo – Basketball Scoreboard System](https://borsimir.github.io/Basketball-Scoreboard-System/controlpanel.html)**

A comprehensive, professional-grade web-based basketball scoreboard system with real-time synchronization, automatic backups, and intuitive game management features.

## 🌟 Features
### Core Functionality
- **Real-time Score Management** - Track scores for both teams with +1, +2, +3 point buttons
- **Dual Clock System** - Game clock (10 minutes) and shot clock (24 seconds) with precise timing
- **Team Management** - Editable team names with dynamic display updates
- **Foul & Timeout Tracking** - Monitor team fouls and timeouts with automatic penalty alerts
- **Quarter Management** - Progress through quarters with automatic resets

### Advanced Features
- **Real-time Synchronization** - Control panel and scoreboard display sync instantly using BroadcastChannel API
- **Professional Audio Cues** - Buzzer sounds for game events and substitutions
- **Automatic Backups** - Game data automatically saved at critical moments
- **Visual Alerts** - Color-coded warnings for low time situations
- **Offline Capability** - Works without internet after initial loading

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Edge, Safari)
- No additional software installation required

### Setup Instructions

1. **Download or Clone the Repository**
   ```bash
   git clone https://github.com/BORSIMIR/basketball-scoreboard
   cd basketball-scoreboard
   ```

2. **Launch the System**
   - Open `controlpanel.html` in your web browser
   - The system is now ready to use!

3. **Open the Scoreboard Display**
   - Click "Open Scoreboard" button in the control panel
   - Position the scoreboard window on a secondary display for spectators

## 📁 File Structure

```
Basketball-Scoreboard-System-main/
├── controlpanel.html          # Main control interface
├── public/
│   ├── scoreboard.html        # Spectator display
│   ├── script.js              # Core game logic
│   ├── style.css              # Styling
│   ├── sweetalert2.min.js     # Alert dialogs
│   ├── sweetalert2.min.css    # Alert styling
│   ├── basketball_buzzer_improved.mp3        # Game buzzer sound
│   └── basketball_substitution_buzzer.mp3    # Substitution sound
├── usermanual.html            # Comprehensive user guide
└── README.md                  # This file
```

## 🎮 How to Use

### Initial Setup
1. **Set Team Names**: Click on "HOME" or "AWAY" to edit team names
2. **Configure Display**: Open the scoreboard window for spectators
3. **Start Game**: Begin with the game clock controls

### During the Game

#### Score Management
- Use **+1**, **+2**, **+3** buttons to add points
- Use **-1** button for score corrections
- Scores update instantly on both displays

#### Clock Control
- **Game Clock**: 10-minute quarters with start/pause/reset controls
- **Shot Clock**: 24-second countdown with 14-second reset option
- **Fine Adjustments**: ±1 second and ±1 minute buttons for precise timing

#### Fouls & Timeouts
- Track team fouls with automatic penalty alerts at 5 fouls
- Manage timeouts (7 per team) with one-click buttons
- All changes sync immediately to scoreboard display

#### Game Flow
- **Timeout**: Pauses both clocks simultaneously
- **Substitution**: Plays audio cue for player changes
- **Next Quarter**: Advances quarter and resets clocks/fouls
- **Save Game**: Export current game data to file

## 🔧 Technical Details

### Architecture
- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Real-time Sync**: BroadcastChannel API for instant updates
- **Audio**: HTML5 Audio API for professional sound effects
- **Storage**: Session-based with manual export options
- **File Management**: File System Access API with fallback to downloads

### Browser Compatibility
| Feature | Chrome | Firefox | Edge | Safari |
|---------|--------|---------|------|--------|
| Core Functions | ✅ | ✅ | ✅ | ✅ |
| Real-time Sync | ✅ | ✅ | ✅ | ✅ |
| Audio Playback | ✅ | ✅ | ✅ | ✅ |
| File Saving | ✅ | ✅ | ✅ | ⚠️* |

*Safari has limited File System Access API support

### Key Technologies
- **BroadcastChannel API**: Enables real-time communication between control panel and scoreboard
- **RequestAnimationFrame**: Provides smooth, 60fps clock updates
- **SweetAlert2**: Beautiful confirmation dialogs and alerts
- **CSS Grid/Flexbox**: Responsive, professional layout design

## 📊 Game Data Management

### Automatic Backups
The system automatically saves game data during:
- Last 5 minutes of any quarter
- End of each quarter
- Critical game events

### File Format
Saved files include:
- Complete game state (scores, fouls, timeouts)
- Clock status and remaining time
- Team information and quarter details
- Timestamp and game status
- Developer credits and system info

### File Naming Convention
```
game_data_YYYYMMDD_Q[quarter]_[HOME_TEAM]_VS_[AWAY_TEAM].txt
```

## 🎨 Visual Features

### Color-Coded Alerts
- **Game Clock**: Yellow at 2:00, Red at 1:00 remaining
- **Shot Clock**: Yellow at 10 seconds, Red at 5 seconds
- **Precision Display**: Milliseconds shown in final seconds

### Professional Layout
- Clean, stadium-style design
- High contrast for visibility
- Responsive design adapts to different screen sizes
- Intuitive button placement for quick access

## 🔊 Audio System

### Sound Effects
- **Game Buzzer**: Played when time expires
- **Substitution Sound**: Unique audio cue for player changes
- **Automatic Triggers**: Sounds play at appropriate game events

### Audio Management
- HTML5 Audio with error handling
- Automatic reset for repeated playback
- Browser permission handling for seamless operation

## 🛠️ Troubleshooting

### Common Issues

**Scoreboard not updating**
- Ensure both windows are from the same browser session
- Refresh both control panel and scoreboard windows
- Check that JavaScript is enabled

**Audio not playing**
- Allow audio permissions when prompted by browser
- Check system volume and browser audio settings
- Refresh page and interact with controls to enable audio

**Buttons not responding**
- Refresh the control panel page
- Check browser console for JavaScript errors
- Ensure you're using a supported browser version

### Browser Permissions
The system may request permissions for:
- Audio playback (for buzzer sounds)
- File system access (for saving game data)

## 📱 Mobile Support

While optimized for desktop use, the system includes:
- Responsive design elements
- Touch-friendly button sizes
- Adaptive layouts for smaller screens

**Note**: For optimal experience, use on desktop/laptop with external display for scoreboard.

## 🤝 Contributing

Contributions are welcome! Please feel free to:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

### Development Setup
1. Clone the repository
2. Open files in your preferred code editor
3. Use a local web server for testing (e.g., Live Server extension)
4. Test across multiple browsers

## 📄 License

This project is open source. Feel free to use, modify, and distribute according to your needs.

## 📞 Support & Contact

**Developer**: Dale Andrew Abila  
**GitHub**: [@BORSIMIR](https://github.com/BORSIMIR)  
**Repository**: [Basketball Scoreboard System](https://github.com/BORSIMIR/Basketball-Scoreboard-System)

---

## 🎯 System Requirements

### Minimum Requirements
- Modern web browser with JavaScript enabled
- Audio support for game sounds
- Screen resolution: 1024x768 or higher

### Recommended Setup
- Dual monitor setup (control panel + scoreboard display)
- Dedicated browser window for scoreboard
- Stable system for continuous operation during games

---

**Made with ❤️ for basketball enthusiasts and game officials**

*Professional scoreboard management made simple and reliable*
