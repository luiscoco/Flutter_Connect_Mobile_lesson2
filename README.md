# How to connect your mobile phone to your laptop for debugging a Flutter application

https://developer.android.com/tools/adb#wireless-adb-android-11

To install and set up **Android Debug Bridge (adb)** for debugging a Flutter application on your mobile phone, follow these steps:

## 1. Step 1: Install Android Studio

Download and Install Android Studio: Download Android Studio from the official Android developer website

https://developer.android.com/studio

![image](https://github.com/luiscoco/Flutter_Connect_Mobile_lesson2/assets/32194879/f86926a5-a306-4c66-85d8-0f808879eee9)

Install Android SDK: During the installation, ensure that the Android SDK is installed

We press in the three dots button and we select the option **SDK Manager**

![image](https://github.com/luiscoco/Flutter_Connect_Mobile_lesson2/assets/32194879/dcff12f6-465d-4a56-83dc-5ccbd3e03778)

We have to select the **SDK Tools** tab and then install **Android SDK Command-Line Tools**

![image](https://github.com/luiscoco/Flutter_Connect_Mobile_lesson2/assets/32194879/f55270bf-8ebf-4e78-b465-56d883f7a20f)

## 2. Step 2: Set Up adb

Open Android Studio:

Launch Android Studio and go to the **SDK Manager**

Navigate to **Configure > SDK Manager**

Install SDK Platform Tools:

In the SDK Manager, go to the **SDK Tools** tab

Check the box for **Android SDK Platform-Tools**

![image](https://github.com/luiscoco/Flutter_Connect_Mobile_lesson2/assets/32194879/8c4a8152-757d-4c23-b967-51ca86c927ed)

Click **OK** to install the package

## 3. Step 3: Add adb to System PATH

Find adb Location:

The **adb** executable is located in the platform-tools directory inside the Android SDK directory

Common default paths:

**Windows: C:\Users\<Your-Username>\AppData\Local\Android\Sdk\platform-tools**

macOS: ~/Library/Android/sdk/platform-tools

Linux: ~/Android/Sdk/platform-tools

**Add to PATH**:

Windows:

Open Control **Panel > System and Security > System > Advanced system settings**

Click on **Environment Variables**

Under **System variables**, find the **Path** variable, and click **Edit**

Click New and add the path to the platform-tools directory

Click OK to save the changes

**C:\Users\luisc\AppData\Local\Android\Sdk\platform-tools**

![image](https://github.com/luiscoco/Flutter_Connect_Mobile_lesson2/assets/32194879/e8decfb6-d6cf-4b33-86cf-188cf60fcc3a)

## 4. Step 4: Enable USB Debugging on Your Mobile Phone

Enable Developer Options:

On your Android phone, go to **Settings > About** phone

**Tap Build number seven times** to **enable Developer** options

Enable USB Debugging:

Go to **Settings > System > Developer** options

Enable **USB debugging**

## 5. Step 5: Verify adb Installation

Connect Your Phone:

Connect your Android phone to your computer using a **USB cable**

**Verify adb Connection**:

Open a terminal (Command Prompt on Windows, Terminal on macOS/Linux)

Run the following command:

```
adb devices
```

You should see your device listed. If prompted on your phone, **authorize the connection**

## 6. Step 6: Debug Flutter Application

Open your Flutter project

Run the Flutter application:

In the terminal, navigate to your Flutter project directory

Run the following command to start debugging on your connected device:

```
flutter run
```

Your Flutter application should now be running on your **mobile phone**, and you can use **adb** for debugging purposes




