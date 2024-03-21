### 할당 순서

1. Android device or emulator
2. iOS simulator
3. iOS device

## Initial project setup (all platforms)

- eas build:configure
- Would you like to automatically create an EAS project for @~~? YES
- Which platforms would you like to configure for EAS Build? » All

## Make a development build for an Android device/ emulator

- npx expo install expo-location expo-dev-client expo-updates
- eas build --profile development --platform android
- What would you like your Android application id to be? » com.tonyworld.myexpoapp
- Generate a new Android Keystore? y
- Install and run the Android build on an emulator? ... no
  - no해서 직접 기기에서 보기

## Make a development build for an iOS simulator

- eas.json에서 build > development에서 ios simulator: true하기

```
"ios": {
  "simulator": true
}
```

- eas build --profile development --platform ios
- What would you like your iOS bundle identifier to be? » com.tonyworld.myexpoapp

Make a development build for an iOS device
Conclusion
