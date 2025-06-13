# 🚀 BAR Replay Analyzer

[![Firebase](https://img.shields.io/badge/Firebase-v10.7.1-orange.svg)](https://firebase.google.com/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Beta-yellow.svg)]()

**Community-driven replay analyzer for Beyond All Reason players** - Track performance, analyze strategies, improve your game with AI-powered insights and persistent data storage.

![BAR Replay Analyzer](https://via.placeholder.com/800x400/1a1a2e/4CAF50?text=BAR+Replay+Analyzer+Demo)

## ✨ Features

### 🔐 **Authentication System**
- **Email/Password** registration and login
- **Google Sign-In** integration
- **Secure user sessions** with Firebase Auth
- **Automatic profile creation** for new users

### 📊 **Advanced Analytics**
- **APM (Actions Per Minute)** tracking with timeline charts
- **Build Order Efficiency** analysis
- **Resource Management** optimization insights
- **Unit Composition** breakdown (Bots, Vehicles, Aircraft)
- **Map-specific performance** tracking
- **Faction win rates** and preferences

### 💾 **Persistent Data Storage**
- **User profiles** with comprehensive statistics
- **Replay history** with detailed analysis results
- **Progress tracking** over time
- **Personal averages** and performance metrics
- **Firestore Database** for reliable cloud storage

### 🎨 **Modern UI/UX**
- **Glassmorphism design** with beautiful gradients
- **Responsive layout** for desktop and mobile
- **Drag & drop** file upload with progress tracking
- **Interactive charts** and real-time data visualization
- **Dark theme** optimized for gaming

### 🚀 **Smart Features**
- **AI-based gameplay analysis** and improvement suggestions
- **Performance comparisons** with players of similar rank
- **Trend identification** and progress visualization
- **File validation** and error handling
- **Demo mode** for testing without uploads

## 🛠️ Tech Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Backend**: Firebase (Auth, Firestore)
- **Database**: Cloud Firestore (NoSQL)
- **Charts**: HTML5 Canvas with custom rendering
- **Authentication**: Firebase Auth with Google OAuth
- **Hosting**: Firebase Hosting (optional)

## 🚀 Quick Start

### Prerequisites
- Modern web browser with JavaScript enabled
- Firebase project with Authentication and Firestore enabled

### Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/bar-replay-analyzer.git
   cd bar-replay-analyzer
   ```

2. **Configure Firebase**
   - Create a new Firebase project at [console.firebase.google.com](https://console.firebase.google.com)
   - Enable **Authentication** → **Email/Password** and **Google** sign-in
   - Enable **Firestore Database** in test mode
   - Copy your Firebase config and replace it in `bar_replay_analyzer.html` (line 318-325)

3. **Open the app**
   ```bash
   # Option 1: Direct file access
   open bar_replay_analyzer.html
   
   # Option 2: Local server (recommended)
   python -m http.server 8000
   # Then visit: http://localhost:8000
   ```

### Firebase Configuration
Replace the Firebase config in the HTML file:
```javascript
const firebaseConfig = {
    apiKey: "your-api-key",
    authDomain: "your-project.firebaseapp.com",
    projectId: "your-project-id",
    storageBucket: "your-project.appspot.com",
    messagingSenderId: "123456789",
    appId: "your-app-id",
    measurementId: "G-XXXXXXXXXX"
};
```

## 📁 Project Structure

```
bar-replay-analyzer/
├── bar_replay_analyzer.html    # Main application file
├── README.md                   # Project documentation
└── .gitignore                 # Git ignore rules
```

## 🎮 Usage

1. **Create Account**: Register with email/password or Google Sign-In
2. **Upload Replay**: Drag & drop or select `.sdfz` or `.replay` files (max 50MB)
3. **View Analysis**: Get detailed insights on your gameplay performance
4. **Track Progress**: Monitor your improvement over time with persistent statistics
5. **Compare Performance**: See how you stack up against your historical averages

## 📊 Data Structure

### User Profile
```javascript
{
  email: "player@example.com",
  displayName: "PlayerName",
  totalGames: 42,
  totalPlayTime: 12680, // seconds
  averageAPM: 127,
  winRate: 68, // percentage
  favoriteMap: "Comet Catcher",
  favoriteFaction: "Cortex",
  createdAt: timestamp,
  lastLogin: timestamp
}
```

### Replay Analysis
```javascript
{
  filename: "epic_game.sdfz",
  mapName: "Red River",
  faction: "Armada",
  gameDuration: "23:47",
  apm: 142,
  buildEfficiency: 87,
  resourceEff: 73,
  unitsBuilt: {
    bots: 34,
    vehicles: 45,
    aircraft: 21
  },
  result: "win",
  createdAt: timestamp
}
```

## 🔮 Roadmap

### Phase 1: Core Features ✅
- [x] Authentication system
- [x] File upload and validation
- [x] Basic analysis display
- [x] User profiles and statistics
- [x] Firestore integration

### Phase 2: Enhanced Analytics 🚧
- [ ] Real replay file parsing
- [ ] Advanced build order analysis
- [ ] Heat maps and positioning analysis
- [ ] Comparison with pro players
- [ ] Detailed unit micro analysis

### Phase 3: Social Features 📋
- [ ] Replay sharing and community
- [ ] Leaderboards and rankings
- [ ] Team analysis for multiplayer games
- [ ] Tournament integration
- [ ] Coaching recommendations

### Phase 4: AI Integration 📋
- [ ] Machine learning game outcome prediction
- [ ] Personalized improvement suggestions
- [ ] Strategy recommendations
- [ ] Automated replay highlights
- [ ] Performance anomaly detection

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Beyond All Reason** community for inspiration
- **Firebase** for providing excellent backend services
- **Contributors** who help improve the analyzer
- **Players** who provide feedback and testing

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/bar-replay-analyzer/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/bar-replay-analyzer/discussions)
- **Discord**: [BAR Community Discord](https://discord.gg/beyond-all-reason)

## 🌟 Show Your Support

If this project helps you improve your BAR gameplay, please ⭐ star the repository!

---

**Made with ❤️ for the Beyond All Reason community**
