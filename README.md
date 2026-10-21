# Happy Kids Learning (Expo starter)

A bilingual English/Hindi educational app prototype for Android/iOS built with React Native and Expo.

## Included
- Home screen with language toggle (English/Hindi)
- Age group selector (5–7, 8–11, 12–15)
- 8 quiz/game categories
- Multiple-choice questions with immediate feedback
- Star rewards, best scores, completed-game counter
- Progress saved locally with AsyncStorage
- Progress reset confirmation

## Run locally
1. Install Node.js (LTS) and Git if needed.
2. Extract this folder and open a terminal inside it.
3. Run `npm install`
4. Run `npx expo start`
5. Install Expo Go on your Android phone and scan the QR code, or use an Android emulator.

## Build an Android APK
For a cloud build, create an Expo account and configure EAS:
1. `npm install -g eas-cli`
2. `eas login`
3. `eas build:configure`
4. In `eas.json`, use an APK build profile, for example:
   ```json
   {
     "build": {
       "preview": {
         "distribution": "internal",
         "android": { "buildType": "apk" }
       }
     }
   }
   ```
5. This project already includes `eas.json` with a preview APK profile.
5. Run `eas build -p android --profile preview`

This source bundle is a starter prototype, not a compiled APK. Test the app and install dependencies before distributing it. Questions are sample content and can be expanded per age group.
