# NutriResilience AI – Android Project

This project packages the supplied **NutriResilience AI – Prototype.html** as an Android app using a native Android WebView container.

## Included
- Offline HTML app bundled inside the APK
- JavaScript enabled
- LocalStorage enabled for check-in data
- English / Kiswahili support from the original prototype
- Nutrition meal planner
- Wellbeing check-in and breathing exercise
- `tel:` links open the phone dialer
- Portrait phone layout
- App theme and launcher artwork
- GitHub Actions workflow for building an APK without Android Studio

## Phone-only build using GitHub
1. Download and extract this ZIP.
2. Create a new GitHub repository, for example `NutriResilienceAI-Android`.
3. Upload **all files and folders** from this project to the repository.
4. Open **Actions** in the repository.
5. Select **Build Android APK**.
6. Tap **Run workflow** (or push to the `main` branch).
7. When the workflow finishes, open the workflow run and download **NutriResilience-AI-debug-apk**.
8. Extract/download `app-debug.apk` and install it on your Android phone.

## Android Studio build
Open the project root (the folder containing `settings.gradle`) in Android Studio, allow Gradle sync, then use **Build > Generate App Bundles or APKs > Generate APKs**.

## Release APK
For a public/conference release, create a signing keystore and configure a `release` signing configuration. Do not put a private keystore or passwords directly into GitHub source code. Store signing secrets in GitHub Actions Secrets.

## Before public launch
The supplied prototype contains placeholder referral text and says phone/referral numbers should be verified before launch. Verify all health/referral information and emergency contacts for the intended deployment area before presenting it as a production service.
