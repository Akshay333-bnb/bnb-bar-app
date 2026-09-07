# Barefoot & Beyond Bar Inventory — One-Click APK Build

This repository builds the Android APK automatically using GitHub Actions. You do **not** need Android Studio or Gradle installed on your computer.

## One-click setup

1. Create a new GitHub repository (for example `barefoot-bar-inventory`).
2. Upload all files and folders from this project into the repository, keeping `.github/workflows/build-apk.yml` in place.
3. Open the repository's **Actions** tab.
4. Select **Build Android APK**.
5. Click **Run workflow**.
6. When the workflow finishes, open the completed run and download the artifact named **Barefoot-Beyond-Bar-Inventory-APK**.
7. The downloaded ZIP contains `app-debug.apk`, which can be installed on an Android phone.

A push to the `main` branch also builds the APK automatically.

## App

- App name: Barefoot & Beyond Bar Inventory
- Application ID: `com.barefootandbeyond.inventory`
- Minimum Android version: Android 6.0 / API 23
- Target SDK: 35
- Build: debug APK (suitable for installation/testing)

## Important

This workflow creates an **unsigned debug APK** for direct installation/testing. For Google Play distribution, a signed release build and Play App Bundle (`.aab`) should be added later.
