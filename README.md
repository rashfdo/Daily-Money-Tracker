# Daily Money Tracker (Android)

Sinhala/English offline income and expense tracker for LKR.

## Features
- Offline SQLite storage on the phone
- Income and expense entries with date, category and note
- Monthly income, expense and balance summary
- Edit and delete transactions
- JSON backup export and restore using Android document picker
- Sinhala / English language toggle

## Build APK on GitHub (no Android Studio needed)
1. Create a GitHub repository.
2. Extract this ZIP.
3. Upload the **contents inside this project folder** to the repository root. Make sure `.github/workflows/android-apk.yml` is included. On GitHub's upload page, hidden folders may need to be included by selecting the whole extracted contents on a computer; if using a phone, create the workflow file separately at the exact path.
4. Open the repository's **Actions** tab.
5. Select **Build Daily Money Tracker APK** and run the workflow, or wait for the push workflow.
6. When the run succeeds, open it and download `DailyMoneyTracker-debug-apk` under **Artifacts**.
7. Extract the downloaded artifact ZIP and install `app-debug.apk` on the Android phone. Allow installation from that browser/file manager if Android asks.

## Build configuration
- Android Gradle Plugin 8.7.3
- Kotlin 2.0.21
- Java/Kotlin JVM target 17
- compileSdk 35
- Gradle 8.9 (provided by the GitHub Actions workflow)

## Data and backup
Transactions are stored in the app's private SQLite database. Uninstalling the app or clearing its storage deletes local data. Export JSON backups regularly and keep them private.
