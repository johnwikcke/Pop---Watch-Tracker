# 🍿 Pop - Watch Tracker

A modern, minimalist Progressive Web App (PWA) for tracking your TV shows, movies, anime, and web series. Built with vanilla HTML, CSS, and JavaScript - no frameworks required!

![Pop Watch Tracker](https://img.shields.io/badge/PWA-Ready-brightgreen) ![License](https://img.shields.io/badge/license-MIT-blue) ![Version](https://img.shields.io/badge/version-2.5.0-orange)

## ✨ Features

### 📱 Core Functionality
- **Track Multiple Content Types**: TV Shows, Movies, Anime, Web Series
- **Episode Management**: Mark episodes as watched/unwatched with visual progress tracking
- **Season Organization**: Organize content by seasons with bulk actions
- **Search & Filter**: Quick search across titles, original titles, and tags
- **Status Categories**: Organize shows by Watching, Planned, Finished, or view All

### 🎨 User Experience
- **Dark/Light Theme**: Automatic system theme detection with manual override
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Progressive Web App**: Install on your device for native app experience
- **Offline Support**: Works without internet connection
- **Touch Optimized**: Long-press context menus and touch-friendly controls

### 📊 Advanced Features
- **Dashboard Analytics**: View detailed statistics about your watching habits
- **Data Management**: Export/Import your data as JSON
- **Poster Support**: Add custom posters via file upload or URL
- **Undo Actions**: Undo recent changes with toast notifications
- **Keyboard Navigation**: Full keyboard accessibility support

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended) ( THIS IS ONLY FOR MOBILE SO IF YOU VIEW FROM PC USE YOU DEV MODE)
Visit the live demo: **[Pop Watch Tracker](https://johnwikcke.github.io/Pop---Watch-Tracker)**

### Option 2: Android App 📱
Get the native Android experience:

1. **Download APK** (coming soon)
2. **Build from source**:
   ```bash
   git clone https://github.com/johnwikcke/Pop---Watch-Tracker.git
   cd Pop---Watch-Tracker/android
   ./gradlew assembleDebug
   ```
3. **Quick setup**: See [ANDROID_SETUP.md](ANDROID_SETUP.md) for 5-minute setup guide

### Option 3: Local Web Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/johnwikcke/Pop---Watch-Tracker.git
   cd Pop---Watch-Tracker
   ```

2. **Open in browser**
   ```bash
   # Using Python (if installed)
   python -m http.server 8000
   
   # Using Node.js (if installed)
   npx serve .
   
   # Or simply open index.html in your browser
   ```

3. **Access the app**
   Open `http://localhost:8000` in your browser

### Option 4: Install as PWA
1. Visit the app in Chrome/Edge/Safari
2. Look for the "Install" button in the address bar
3. Click to install as a native app on your device

## 📖 How to Use

### Adding Your First Show
1. Click the **"+"** button in the header or the "Add Show" button
2. Fill in the show details:
   - **Title**: The show name
   - **Original Title**: Optional original language title
   - **Type**: TV Show, Movie, Anime, or Web Series
   - **Seasons**: Number of seasons (auto-hidden for movies)
   - **Episodes**: Episodes per season
   - **Status**: Planned, Watching, Paused, or Finished
   - **Tags**: Comma-separated tags for organization
   - **Poster**: Upload an image or paste a URL

### Tracking Progress
- **Episode Tracking**: Click episode numbers to mark as watched/unwatched
- **Season Actions**: Use "Mark Complete" to mark entire seasons
- **Bulk Actions**: Right-click (or long-press) episodes for context menu
- **Auto Status**: Status automatically updates based on progress

### Managing Your Library
- **Search**: Use the search bar to find shows by title or tags
- **Filter**: Switch between Watching, Planned, Finished, or All tabs
- **Sort**: Choose from Recently Updated, Alphabetical, or Progress sorting
- **Edit**: Click any show to view details and edit information

### Data Management
1. **Export Data**: Settings → Export Data (downloads JSON file)
2. **Import Data**: Settings → Import Data (upload JSON file)
3. **Dashboard**: View detailed statistics about your watching habits

## 🛠️ Technical Details

### Built With
- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Modern CSS with CSS Grid, Flexbox, and CSS Variables
- **Vanilla JavaScript**: No frameworks - pure ES6+ JavaScript
- **PWA Technologies**: Service Worker, Web App Manifest, Local Storage
- **Android**: Native WebView wrapper for Android devices

### Platform Support
- ✅ Firefox 75sers**: Chrome 80+, Firefox 75+, Safari 13+, Edge 80+
- ✅ **Mobile Web**:afari, Chrome Mobile, Samsung Internet
- ✅ **Android**: Native Android app (API 21+, Android 5.0+)
- ✅ **PWA**: Installable on all modern platforms

### Storage
- **Local Storage**: All data stored locally in your browser
- **No Server Required**: Completely client-side application
- **Privacy First**: Your data never leaves your device

## 🎯 Roadmap

### Upcoming Features
- [ ] **Sync Support**: Optional cloud sync across devices
- [ ] **Advanced Analytics**: More detailed viewing statistics
- [ ] **Recommendations**: Suggest shows based on viewing history
- [ ] **Social Features**: Share progress with friends
- [ ] **API Integration**: Fetch show data from TMDB/TVDB
- [ ] **Custom Categories**: Create custom status categories
- [ ] **Watch Time Tracking**: Track total time spent watching

### Completed ✅
- [x] Basic show tracking
- [x] Episode management
- [x] PWA support
- [x] Dark/Light themes
- [x] Data export/import
- [x] Dashboard analytics
- [x] Poster support
- [x] Search functionality
- [x] Responsive design

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Reporting Issues
1. Check existing [issues](https://github.com/johnwikcke/pop-watch-tracker/issues)
2. Create a new issue with:
   - Clear description of the problem
   - Steps to reproduce
   - Expected vs actual behavior
   - Browser and device information

### Submitting Changes
1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Commit** your changes: `git commit -m 'Add amazing feature'`
4. **Push** to the branch: `git push origin feature/amazing-feature`
5. **Open** a Pull Request

### Development Setup
```bash
# Clone your fork
git clone https://github.com/johnwikcke/pop-watch-tracker.git
cd pop-watch-tracker

# Create a feature branch
git checkout -b feature/your-feature-name

# Make your changes and test locally
# Open index.html in your browser

# Commit and push
git add .
git commit -m "Description of your changes"
git push origin feature/your-feature-name
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Design Inspiration**: Modern PWA design patterns
- **Icons**: SVG icons from Feather Icons
- **Typography**: System font stack for optimal performance
- **Color Palette**: Carefully chosen for accessibility and aesthetics

## � Docpumentation

### Development Guides
- **[ANDROID_GUIDE.md](ANDROID_GUIDE.md)** - Complete Android development guide
- **[ANDROID_SETUP.md](ANDROID_SETUP.md)** - Quick 5-minute Android setup

### External Resources
- [Android WebView Documentation](https://developer.android.com/guide/webapps/webview)
- [PWA Documentation](https://web.dev/progressive-web-apps/)
- [Google Play Console Help](https://support.google.com/googleplay/android-developer/)

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/johnwikcke/Pop---Watch-Tracker/issues)
- **Discussions**: [GitHub Discussions](https://github.com/johnwikcke/Pop---Watch-Tracker/discussions)
- **Email**: saymynamejk0@gmail.com

## 🌟 Show Your Support

If you find this project helpful, please consider:
- ⭐ **Starring** the repository
- 🐛 **Reporting** bugs and issues
- 💡 **Suggesting** new features
- 🔄 **Sharing** with friends and colleagues

---

**Made with ❤️ by [Non Popular Point](https://github.com/johnwikcke)**

*Keep track of what you watch, discover what you love!* 🍿✨
