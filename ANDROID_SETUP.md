# 🚀 Quick Android Setup Guide

This guide will help you quickly set up the Android version of Pop Watch Tracker.

## 📋 Prerequisites

- **Android Studio** (latest version recommended)
- **Java Development Kit (JDK)** 8 or higher
- **Android SDK** (API level 21 or higher)
- **Git** (for cloning the repository)

## ⚡ Quick Start (5 Minutes)

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/pop-watch-tracker.git
cd pop-watch-tracker
```

### Step 2: Copy Web Assets
```bash
# Create assets directory
mkdir -p android/app/src/main/assets

# Copy your HTML file
cp index.html android/app/src/main/assets/

# If you have separate CSS/JS files, copy them too
# cp -r css android/app/src/main/assets/
# cp -r js android/app/src/main/assets/
```

### Step 3: Open in Android Studio
1. Open Android Studio
2. Click "Open an existing project"
3. Navigate to the `android` folder in your cloned repository
4. Click "OK"

### Step 4: Build and Run
1. Wait for Gradle sync to complete
2. Connect an Android device or start an emulator
3. Click the "Run" button (green play icon)
4. Your app should install and launch!

## 📱 Testing Your App

### On Physical Device
1. Enable "Developer Options" on your Android device
2. Enable "USB Debugging"
3. Connect via USB
4. Select your device in Android Studio
5. Click "Run"

### On Emulator
1. In Android Studio, go to Tools → AVD Manager
2. Create a new Virtual Device
3. Choose a device definition (e.g., Pixel 4)
4. Select a system image (API 30+ recommended)
5. Click "Finish" and start the emulator

## 🎨 Customization

### App Icon
Replace the default icons in:
- `android/app/src/main/res/mipmap-*/ic_launcher.png`

### App Name
Edit `android/app/src/main/res/values/strings.xml`:
```xml
<string name="app_name">Your App Name</string>
```

### Colors
Edit `android/app/src/main/res/values/colors.xml`:
```xml
<color name="primary">#YourColor</color>
```

### Package Name
1. In Android Studio, right-click the package folder
2. Select "Refactor" → "Rename"
3. Choose "Rename package"
4. Update `applicationId` in `build.gradle`

## 🔧 Advanced Configuration

### Enable File Uploads
The app already supports file uploads for poster images. No additional setup needed!

### Add Splash Screen
The splash screen is already configured. To customize:
1. Edit `android/app/src/main/res/drawable/splash_background.xml`
2. Replace the logo with your own

### Performance Optimization
The WebView is already optimized with:
- Hardware acceleration enabled
- JavaScript optimization
- Memory management
- Caching enabled

## 📦 Building Release APK

### Debug Build (for testing)
```bash
cd android
./gradlew assembleDebug
```
APK location: `android/app/build/outputs/apk/debug/`

### Release Build (for distribution)
1. Generate a signing key:
```bash
keytool -genkey -v -keystore my-release-key.keystore -alias alias_name -keyalg RSA -keysize 2048 -validity 10000
```

2. Add to `android/app/build.gradle`:
```gradle
android {
    signingConfigs {
        release {
            storeFile file('my-release-key.keystore')
            storePassword 'your_password'
            keyAlias 'alias_name'
            keyPassword 'your_password'
        }
    }
    buildTypes {
        release {
            signingConfig signingConfigs.release
        }
    }
}
```

3. Build release APK:
```bash
./gradlew assembleRelease
```

## 🐛 Troubleshooting

### Common Issues

**WebView not loading:**
- Check that `index.html` is in `assets` folder
- Verify JavaScript is enabled in MainActivity

**File uploads not working:**
- Ensure storage permissions are granted
- Check that WebChromeClient is properly set

**App crashes on startup:**
- Check Logcat for error messages
- Verify all dependencies are properly added

**Build errors:**
- Clean and rebuild: `./gradlew clean build`
- Update Android Studio and SDK tools
- Check Gradle version compatibility

### Debug Tools

**Enable WebView debugging:**
```java
WebView.setWebContentsDebuggingEnabled(true);
```
Then use Chrome DevTools at `chrome://inspect`

**View logs:**
```bash
adb logcat | grep "PopWatchTracker"
```

## 📱 Publishing to Google Play

### Prepare for Release
1. **Test thoroughly** on multiple devices
2. **Optimize APK size** using R8/ProGuard
3. **Create store assets**:
   - App icon (512x512)
   - Feature graphic (1024x500)
   - Screenshots (phone and tablet)
   - App description

### Upload to Play Console
1. Create developer account at [Google Play Console](https://play.google.com/console)
2. Create new app
3. Upload APK/AAB file
4. Fill in store listing details
5. Set content rating and pricing
6. Submit for review

## 🔄 Updating Your App

### Update Web Content
1. Modify `index.html` in the assets folder
2. Increment `versionCode` in `build.gradle`
3. Build new APK
4. Test and deploy

### Add New Features
1. Modify MainActivity.java for native features
2. Update permissions in AndroidManifest.xml if needed
3. Test thoroughly
4. Update version and build

## 💡 Pro Tips

1. **Test on real devices** - Emulators don't always reflect real performance
2. **Optimize images** - Compress assets to reduce APK size
3. **Handle offline mode** - Your HTML app already supports this!
4. **Monitor performance** - Use Android Studio's profiler tools
5. **Keep it updated** - Regular updates improve user retention

## 🆘 Need Help?

- **GitHub Issues**: [Create an issue](https://github.com/yourusername/pop-watch-tracker/issues)
- **Email**: saymynamejk0@gmail.com
- **Android Documentation**: [developer.android.com](https://developer.android.com)

---

**Happy coding! 🎉**