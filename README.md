# Land of Jail – Auto Hunter (prototype source)

This is an Android Studio project scaffold for a Level 30 Frenzied Fugitive helper.

## Current status
- Android app shell and Accessibility Service configuration are included.
- ML Kit text recognition is wired to inspect screenshots and detect the exact Level 30 target label.
- The prototype does **not** tap Search, ATK, or March. It is deliberately detection-only until the game's changing screens, screen scaling, and return-to-prison flow are validated on the actual phone.
- It has not been compiled or device-tested in this environment.

## Build
Open this folder in Android Studio (Giraffe or newer), allow Gradle sync, then Build > Build Bundle(s) / APK(s) > Build APK(s).

Requires Android API 30+ because it uses AccessibilityService screenshot capture. Enable the service manually in Android Settings. Only use it while the game is open and stop it at any time.

## Next calibration needed
Test on the target phone: confirm that the game UI text is visible to OCR on (1) the search panel, (2) the fugitive result popup, (3) the troop deployment screen, and (4) the march/return state. Do not enable automatic March until these states are reliably distinguished.
