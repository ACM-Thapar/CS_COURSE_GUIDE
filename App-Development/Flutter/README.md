<a href="https://flutter.dev/">
  <h1 align="center">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://storage.googleapis.com/cms-storage-bucket/6e19fee6b47b36ca613f.png">
      <img alt="Flutter" src="https://storage.googleapis.com/cms-storage-bucket/c823e53b3a1a7b0d36a9.png">
    </picture>
  </h1>
</a>

Flutter is Google's SDK for crafting beautiful, fast user experiences for
mobile, web, and desktop from a single codebase. Flutter works with existing
code, is used by developers and organizations around the world, and is free and
open source.

## About Flutter

Flutter will help you create beautiful, fast apps, with a productive,
extensible and open development model, whether you're targeting iOS or Android,
web, Windows, macOS, Linux or embedding it as the UI toolkit for a platform of
your choice.

## Table of Contents

- [Documentation](#documentations)
- [Installation](#installation)
  - [Android Studio For Android](#android-setup)
  - [Xcode For IOS](#ios-setup)
  - [Add Flutter To VS Code](#vs-code-setup)
  - [Android Emulator](#android-emulator)
  - [IOS Emulator](#ios-emulator)
- [Create Flutter App](#create-flutter-app)

- [Important Packages](#packages)

  - [Fonts](#fonts)
  - [Images](#images)
  - [HTTP(For API Integration)](#api-integration)
  - [Routing](#routing)
  - [File, Path Providers ](#files)
  - [Local Storage](#local-storage)
  - [WebView](#webview)
  - [Firebase](#firebase)
  - [Other Important Packages](#other-important-packages)

- [State Management Tools](#state-management)
- [Popular Courses](#popular-courses)

## Documentations

> [Flutter Documentation](https://docs.flutter.dev/)

> [Firebase Documentaion](https://docs.flutter.dev/data-and-backend/firebase)

> [Dart Documentation](https://dart.dev/language)

## Installation

- ### Android Setup
  1. Install [Android Studio](https://developer.android.com/studio).
  2. Install [Flutter](https://docs.flutter.dev/get-started/install) File.
  3. Watch [this](https://www.youtube.com/watch?v=BqHOtlh3Dd4) Video to Setup Flutter on Android Studio For Windows.
- ### IOS Setup
  1. Install Latest [Android Studio](https://developer.android.com/studio) and [Flutter](https://docs.flutter.dev/get-started/install) File.
  2. Watch [this](https://www.youtube.com/watch?v=f09c-nw15K8) video to setup Flutter on Android Studio and XCode.
- ### VS Code Setup

  Watch [this](https://youtu.be/BqHOtlh3Dd4?t=1835) video to Setup Your Flutter to Vs Code.

  #### Important Plugins For VS Code

  > Flutter

  > Awesome Flutter Snippets

  > Dart

- ### Android Emulator
  - Watch [this](https://www.youtube.com/watch?v=x_lvdLil0Fk) Video to install ios emulator on Android Studio.
- ### IOS Emulator
  - Watch [this](https://youtu.be/f09c-nw15K8?t=330) Video to install ios emulator on XCode.

## Create Flutter App

1. Create a new app by running the below code on terminal

```
flutter create <app_name>
```

2. Open the generated code on your supported platform.

3. Get latest package version by running

```
flutter pub get
```

4. Then run your flutter app by typing the code given below, the list of `available devices` will be shown, select one of the device.

> If you don't have any virtual device then you can install virtual devices for [Android Studio](https://www.youtube.com/watch?v=x_lvdLil0Fk) or [XCode](https://youtu.be/f09c-nw15K8?t=330).

```
flutter run
```

5. You are good to go now.

## Packages

- ### Fonts

  - Google Fonts

    ```
    flutter pub add google_fonts
    ```

- ### Images

  - #### SVG Images
    ```
    flutter pub add flutter_svg
    ```
  - #### Cached Network Image

    - When You want to show the preview of the image without download whole image from network.

      ```
      flutter pub add cached_network_image
      ```

- ### API Integration

  - #### HTTP

    ```
    flutter pub add http
    ```

    - Import like this in your dart file

      ```
      import 'package:http/http.dart' as http;
      ```

  - #### Dio (Works as http but opitimised provides more features than http )
    ```
    flutter pub add dio
    ```

- ### Routing

  - Auto Route

    - You can read the docs to integrate auto_route from here [link](https://pub.dev/packages/auto_route).

      ```
      flutter pub add auto_route
      ```

- ### Files

  - #### Path Provider

    - Provides path to local directories to store files and image temporarily into the system.

      ```
      flutter pub add path_provider
      ```

  - #### Image Picker

    - Used to pick image from the gallery or from your local storage.

      ```
      flutter pub add image_picker
      ```

  - #### File Picker

    - Used to pick pick files(png,pdf,pptx,txt,csv,xlsx,etc..) from your local storage.

      ```
      flutter pub add file_picker
      ```

- ### Local Storage
  - #### Shared Preferences
    - Used to store data (string,int,double,etc..) to the local storage.
      ```
      flutter pub add shared_preferences
      ```
- ### Webview
  - #### WebView Flutter
    - Used to show any html file or any website inside the app.
      ```
      flutter pub add webview_flutter.
      ```
  - #### Flutter InAppWebview
    - Used to show any html file or any website inside the app.
      ```
      flutter pub add flutter_inappwebview.
      ```
- ### Firebase
  - #### Firebase Core
    - Used to connect your app to firebase.
      ```
      flutter pub add firebase_core.
      ```
  - #### Cloud Fireastore
    - Used to fetch, update or add data to firebase firestore.
      ```
      flutter pub add cloud_firestore.
      ```
  - #### Firebase Storage
    - Used to store files to firebase storage.
      ```
      flutter pub add firebase_storage.
      ```
  - #### Firebase Analytics
    - An app measurement solution that provides insight on app usage and user engagement on Android and iOS.
      ```
      flutter pub add firebase_analytics.
      ```
  - #### Firebase Auth
    - Used to add Auth to your app enabling Android and iOS authentication using passwords, phone numbers and identity providers like Google, Facebook and Twitter, etc.
      ```
      flutter pub add firebase_auth.
      ```
- ### Other Important Packages

  - #### Google Sign In

    - A secure authentication system for signing in with a Google account on Android and iOS.

      ```
      flutter pub add google_sign_in
      ```

  - #### Flutter Toast

    - Used to show toast(floating messages) message in the app.

      ```
      flutter pub add fluttertoast
      ```

## State Management

> ### [Riverpod ](https://riverpod.dev/docs/getting_started) (Recommended)

> ### [Provider](https://pub.dev/packages/provider)

> ### [Bloc](https://github.com/felangel/bloc/blob/master/packages/flutter_bloc/README.md)

## Popular Courses

- ### [Flutter & Dart - The Complete Guide By Maximillian (Udemy)](https://www.udemy.com/share/101rfI3@Xj1QdAtofCrhmCIwwGXoMk9jCMveOJbroCpa514kuyNyFf0sU_8sldGcRJX1xck0SA==/)

- ### [Flutter Tutorial For Begineers (Youtube) ](https://www.youtube.com/watch?v=BiOSCpV-lts)
