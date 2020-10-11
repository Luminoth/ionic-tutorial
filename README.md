# Ionic Tutorial

## Global Setup

* Install Node.js
* npm install -g @ionic/cli native-run cordova-res

## Init Application

* ionic start {name} {template} --type=angular --capacitor

* ionic build
* ionic cap add android
* ionic cap add ios

## Install Dependencies

* npm install @ionic/pwa-elements
  * Edit ```src/main.ts```:

```
import { defineCustomElements } from '@ionic/pwa-elements/loader';

// Call the element loader after the platform has been bootstrapped
defineCustomElements(window);
```

## Running

* ionic serve

## Building

* ionic build
* ionic cap copy

## Android

* Install Android Studio
* Enable KVM
  * https://developer.android.com/studio/run/emulator-acceleration?utm_source=android-studio#vm-linux
* ionic cap open android
* ionic cap run android -l --external

## iOS

* ionic cap open ios
* ionic cap run ios -l --external

## Misc Notes

* Add Ionic to existing Angular app
  * ng add @ionic/angular
* Any time native apps are updated, run ```ionic cap sync```
