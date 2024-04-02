Overview : 
    This documentation provides a guide for developing a Face Authentication mobile application using the Ionic framework with Capacitor. The application utilizes biometric authentication (Face ID or Fingerprint) for user verification.

Prerequisites : 
    Node.js installed on your development machine.
    Basic knowledge of Angular, TypeScript, and HTML/CSS.
    Access to a text editor or IDE (e.g., Visual Studio Code).
    Android Studio and/or Xcode for testing and building the app on Android and iOS, respectively.

Installation

Step 1: Create a New Ionic App 
    npm install -g @ionic/cli
    ionic start my-qr-app blank --type=angular
    :- Replace my-qr-app with your desired project name. This command will create a new Ionic app with a blank template using Angular.

Step 2: Navigate to Your Project Directory
    Navigate into the newly created project directory:
    cd my-qr-app

Step 3: Install Capacitor
    npm install @capacitor/core @capacitor/cli

Step 4: Initialize Capacitor
    npx cap init

Step 5: Add Platforms
    npx cap add android
    npx cap add ios

Step 6: Install Additional Packages
    npm install capacitor-native-biometric

Step 7: Sync Your Project with Capacitor
    npx cap sync

Step 8: Verify Installation
    ionic serve

Android Configuration: 
    Ensure the following permission is added in the AndroidManifest.xml:
        <uses-permission android:name="android.permission.USE_BIOMETRIC" />

iOS Configuration:
    Ensure the following usage description key is added in the Info.plist file:
    <key>NSFaceIDUsageDescription</key>
    <string>For an easier and faster login.</string>

Conclusion :
    Congratulations! You have successfully set up your Ionic project for Face Authentication using Capacitor. You can now proceed with developing and customizing your app according to the project requirements.
