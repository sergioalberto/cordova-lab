# Apache Cordova Lab
Examples to create hybrids app mobiles

## Get Started
```shell
# Installing Cordova
npm install -g cordova
npm install -g n
n 12.18.3

# Create a project
cordova create MyApp
```

## Create the App
```shell
cordova create hello com.example.hello HelloWorld
```

## Add Platforms
```shell
cd MyApp
cordova platform add browser
cordova platform add ios
cordova platform add android
```

## Add plugins
```shell
cordova plugin add cordova-plugin-firebasex
# cordova plugin add cordova-plugin-fcm
```

## Install pre-requisites for building
```shell
cordova requirements

# For iOS on MAC
npm install -g ios-deploy
sudo gem install cocoapods

# For Android on MAC
export JAVA_HOME=$(/usr/libexec/java_home -v 1.8)
sdk install gradle 7.2
brew install gradle
# Download Android Studio here: https://developer.android.com/studio/index.html#downloads
# Open SDK manager (from Android Studio) and install an Android SDK version
# Open the AVD manager (from Android Studio) and add an emulator
export ANDROID_SDK_ROOT=/Users/sergio.gonzalez/Library/Android/sdk
export ANDROID_HOME=/Users/sergio.gonzalez/Library/Android/sdk
export PATH=$PATH:$ANDROID_SDK_ROOT/platform-tools/
export PATH=$PATH:$ANDROID_SDK_ROOT/cmdline-tools/latest/bin/
export PATH=$PATH:$ANDROID_SDK_ROOT/emulator/
```

## Build the App
```shell
# For all platforms
cordova build
cordova build browser
cordova build ios
cordova build android
```

## Test the App
```shell
cordova run browser
cordova emulate ios
cordova emulate android
cordova run android
```

### Sources
- https://cordova.apache.org/docs/en/10.x/guide/cli/index.html 
- https://lifesaver.codes/answer/no-installed-build-tools-found-install-the-android-build-tools-version-19-1-0-or-higher
- https://medium.com/@carlospcpro/how-to-add-push-notifications-to-your-cordova-app-in-ios-and-android-using-firebase-done-right-4f6c64dc50f0
- https://console.firebase.google.com
- https://github.com/fechanique/cordova-plugin-fcm
