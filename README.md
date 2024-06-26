# How to install Flutter in your laptop and create a Android Virtual Device (AVD) with Android Studio

## 0. Prerequisites

### Hardware requeriments

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/f960ae23-98b7-423d-8738-871a26759a19)

### Software requeriment

Flutter supports 64-bit version of Microsoft **Windows 10 or later**

These versions of Windows should include the required Windows **PowerShell 5 or later**

Install **VSCode** and **Flutter** extension

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/29d7c341-5acc-4d7c-b393-d4a3cc3badb0)

Install **Visual Studio Community Edition**: https://visualstudio.microsoft.com/vs/community/

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/492a6048-177d-446c-8415-c5e00f5ab427)

Install **IntelliJ IDEA Community Edition**: https://www.jetbrains.com/idea/download/?section=windows

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/8e6c12dd-16d1-42d8-9bf5-9fe430fc6e3d)

**Git for Windows 2.27 or later** to manage source code

Install **Android Studio**: https://developer.android.com/studio/install

Upgrade to latest version **Android Studio**

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/562caf90-cd2f-4a4f-88da-e99195f72484)

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/271c198e-f76e-4fc0-9e4d-eb77cdfa9205)

## 1. Start building Flutter native desktop apps on Windows

https://docs.flutter.dev/get-started/install/windows/desktop

To install the Flutter SDK on Windows, follow these steps:

## 1.1. Download the Flutter SDK**

Go to the Flutter official website: Flutter SDK Download

Download the latest stable version of the Flutter SDK

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/64517bd7-7779-49b5-adf9-0de2aec03627)

## 1.2. Extract the Flutter SDK**

Extract the downloaded zip file to a desired location on your computer, for example, **C:\src\flutter**

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/b88372cb-c8a8-43f7-b363-a7a4c5304fca)

## 1.3. Update your PATH environmental variable

Add the flutter\bin directory to your system's PATH environment variable

You can do this by following these steps:

Open the Start Search, type in "env", and select "Edit the system environment variables"

In the System Properties window, click on the Environment Variables button

In the Environment Variables window, under System variables, find the Path variable, select it, and click Edit

Click New and add the path to the flutter\bin directory, for example, **C:\src\flutter\bin**

Click OK to close all windows

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/80508108-12c0-4963-9cd5-c3b0a16057a4)

## 1.4. Run flutter doctor

Open a new command prompt or PowerShell window and run the following command to verify your Flutter installation:

```
flutter doctor
```

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/02e4b898-98f9-4290-8bcf-b1ac823ce7c1)

or 

```
flutter doctor -v
```

This command will check your Flutter environment and display the installation status of dependencies and tools needed to develop Flutter apps

Follow any additional instructions provided by flutter doctor to complete the setup

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/8d2e3463-14e0-44ef-9a71-1756a85ef79e)

![image](https://github.com/luiscoco/Flutter_Installation/assets/32194879/78fd6f09-ee02-4532-99ed-b1714800f8b6)

## 1.5. How to Upgrade Flutter

To check the version of Flutter installed on your system, you can use the following command in your terminal or command prompt:

```
flutter --version
```

This command will display the Flutter version along with other details like the Dart version and the framework version

To upgrade your Flutter installation to the latest version, you can use the following command in your terminal or command prompt:

```
flutter upgrade
```

This command will fetch the latest stable release of Flutter and update your installation

## 1.6. How to uninstall Flutter

### How to uninstall the SDK

Remove the flutter directory: **C:\src\flutter**

### Remove Flutter configuration files

If you don't want to preserve your Flutter configuration, remove the following directories from your home directory:

**%APPDATA%'.flutter-devtools**

### Remove Dart configuration files

If you don't want to preserve your Dart configuration, remove the following directories from your home directory

**%LOCALAPPDATA%'.dartServer**

**%APPDATA%'.dart**

**%APPDATA%'.dart-tool**

## Remove pub package files

If you want to remove Flutter but not Dart, don't complete this section

If you don't want to preserve your pub packages, remove the **.pub-cache** directory from your home directory

## Remove Flutter from your Windows Path variable

To remove Flutter commands from PowerShell, remove Flutter to the **PATH** environment variable

## 1.7. Install Android SDK Command-line Tools and Android SDK Platform-Tools

Run Android Studio and select **More Actions/SDK Manager**

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/6eb3ca8b-b760-4846-ac47-668b4f0f1feb)

Select the menu option **Android SDK Command Line Tools**

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/2ba1b348-c0eb-4e03-b7d6-2ed85c324cd8)

Select the menu option **Android SDK Platform-Tools**

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/09d8a2a5-d60f-42c8-856a-93dbfe9fc8e1)

## 1.8. Install Flutter and Dart plugins in IntelliJ IDEA Community Edition

We first install **Flutter** plugin

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/ceb611ee-8be2-43e9-8977-7f8bf333e024)

Then we install **Dart** plugin

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/5d5c77d4-af84-4833-ab00-d6eafe11c493)

We verify we already installed Flutter and Dart plugins for IntelliJ 

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/d4320e4a-8e57-4c4d-8b3b-856e3fa8bba3)

## 1.9. How to create a new Android Virtual Device (AVD) in Android Studio

We press the three dots button and then we select the option **Virtual Device Manager**

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/afa0ddb8-32b4-4550-9290-9d72144c25e7)

We press the **Create Device** button

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/dd72fa0c-cf61-45ff-a607-5c713e37bd92)

We now have to chose a device definition and press the **Next** button

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/3cdf5725-7401-4b94-a306-862ab70353a1)

We select the **API 34** tab and then we press the **Next** button  

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/e8a70eef-af34-49a3-9a54-2b8f4bbf6d6a)

We press the **Finish** button for creating the mobile device simulator

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/4f66c5bf-a028-4162-b2b9-4328fdddee8d)

We verify the similator was already created pressing the **Launch this AVD in the emulator** button 

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/6569b77f-9784-4ca9-a2eb-a53c203abbfd)

We can see the device is running 

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/1cfdcbb6-f34a-4c31-9f81-b0e0975c63c2)

We can navigat with Google Chrome

![image](https://github.com/luiscoco/Flutter_Installation_lesson1/assets/32194879/07627a36-670f-4eb1-9edd-47d056b374e9)
