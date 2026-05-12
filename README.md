Flutter client for Birdie

This is a minimal Flutter UI that sends an audio file and Google Drive folder links to the Birdie backend, then displays the top matches returned by the server.

Setup

1. Ensure you have Flutter SDK installed.
2. From this directory run:

```bash
flutter pub get
# If you copied only this folder into an existing Flutter project, run `flutter create .` first to generate platform folders.
flutter run
```

Usage

- On the login screen provide any email and password (demo auth).
- On the upload screen pick a .wav or .mp3 file and provide one or more Google Drive folder links (comma-separated). The app will call the backend at http://10.0.2.2:5000 by default (Android emulator host mapping). Adjust the URL in `lib/main.dart` if your backend runs elsewhere.
