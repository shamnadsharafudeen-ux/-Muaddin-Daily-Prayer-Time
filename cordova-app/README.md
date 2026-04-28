# Muaddin Prayer Time App

This is a Cordova-based mobile app for prayer times with adhaan notifications.

## Setup Instructions

1. Ensure Node.js and Cordova are installed:
   ```
   npm install -g cordova
   ```

2. Navigate to the cordova-app directory:
   ```
   cd cordova-app
   ```

3. Add Android platform:
   ```
   cordova platform add android
   ```

4. Add iOS platform (requires macOS):
   ```
   cordova platform add ios
   ```

5. Add icons: Place professional PNG icons in the res/icon/ folders as specified in config.xml.

6. Add the adhaan audio file:
   - Place `adhan.mp3` inside `cordova-app/www/`.

7. Install Cordova plugins in the project:
   ```
   cd cordova-app
   cordova plugin add cordova-plugin-local-notification cordova-plugin-geolocation cordova-plugin-media
   ```

8. Build for Android:
   ```
   cordova build android
   ```
   The APK will be in platforms/android/app/build/outputs/apk/debug/

9. Build for iOS (on macOS):
   ```
   cordova build ios
   ```

## Features
- Prayer times for any city
- Auto adhaan audio at prayer times
- Local notifications for prayers
- Multi-language support
- Professional dark theme
- Responsive design

## Plugins Used
- cordova-plugin-local-notification: For notifications
- cordova-plugin-geolocation: For location detection
- cordova-plugin-media: For audio playback