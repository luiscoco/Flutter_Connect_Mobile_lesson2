# How to connect your mobile phone to your laptop for debugging a Flutter application

https://developer.android.com/tools/adb#wireless-adb-android-11

To install and set up **Android Debug Bridge (adb)** for debugging a Flutter application on your mobile phone, follow these steps:

## 1. Step 1: Install Android Studio

Download and Install Android Studio: Download Android Studio from the official Android developer website

Install Android SDK: During the installation, ensure that the Android SDK is installed

## 2. Step 2: Set Up adb

Open Android Studio:

Launch Android Studio and go to the SDK Manager

Navigate to Configure > SDK Manager

Install SDK Platform Tools:

In the SDK Manager, go to the SDK Tools tab

Check the box for Android SDK Platform-Tools

Click Apply to install the package

## 3. Step 3: Add adb to System PATH

Find adb Location:

The adb executable is located in the platform-tools directory inside the Android SDK directory

Common default paths:

Windows: C:\Users\<Your-Username>\AppData\Local\Android\Sdk\platform-tools

macOS: ~/Library/Android/sdk/platform-tools

Linux: ~/Android/Sdk/platform-tools

**Add to PATH**:

Windows:

Open Control Panel > System and Security > System > Advanced system settings

Click on Environment Variables

Under System variables, find the Path variable, and click Edit

Click New and add the path to the platform-tools directory

Click OK to save the changes




