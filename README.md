# Building an APK from an Expo Project

## Prerequisites
- Ensure you have Node.js installed
- Ensure your project uses Expo SDK 41 or later
- Install the Expo CLI and EAS CLI

```sh
npm install -g expo-cli eas-cli
```

## Step-by-Step Guide

### 1. Navigate to Your Project
Open your terminal and navigate to your Expo project directory.

```sh
cd your-expo-project
```

### 2. Log in to Expo
Make sure you are logged into your Expo account.

```sh
expo login
```

### 3. Configure EAS Build
Run the following command to configure your project for EAS Build.

```sh
eas build:configure
```

### 4. Create a Build for Android
Use the EAS CLI to start a new build for the Android platform. This command will prompt you for some additional information, such as your Android package name.

```sh
# Create aab file for PlayStore
eas build --platform android
# create apk 
eas build -p android --profile preview
```

### 5. Monitor the Build
You can monitor the build process in your terminal or visit the Expo build page provided in the terminal output.

### 6. Download the APK
Once the build is complete, you will receive a URL where you can download the APK file.

## Additional Resources
- [Expo EAS Build Documentation](https://docs.expo.dev/build/introduction/)
- [Expo CLI Installation Guide](https://docs.expo.dev/get-started/installation/)

## Troubleshooting
If you encounter issues during the build process, consult the Expo documentation or seek help from the Expo community.
