# Install Hawk Eye on Android

Download `Hawk-Eye.apk` from this repository's release assets, then open it on the phone. If Android asks, allow installation from the browser or Files app you used and choose Install. This is a development-signed test build for Android 8.0/API 26 or newer with OpenGL ES 3.0 support.

To update an existing Hawk Eye installation, install the APK over the current app. The development signing identity is retained; keeping the app installed preserves its settings and weather key. If Android reports a signature conflict, stop rather than uninstalling and losing saved settings.

## Connect live weather

Open Hawk Eye with an internet connection. The built-in HTTPS weather service connects automatically; no weather key, account or activation step is required. It refreshes while the app is open and retrieves current data after reconnecting.

Look for **Live** or **Delayed**; **Delayed** means one or more source observations are stale. **Offline** means cached weather is being shown. Use **More → Retry weather** if needed. If you previously configured a different service, open **More → Settings** and clear the service address to restore the built-in connection. The optional key field is only for custom private services.

The public weather endpoint serves the configured test location. Server credentials are not included in this download. The APK includes the location's terrain and imagery; this is a fixed test world, not a personal-address setup service.

## Views and checks

Use **Views** for Home, Yard, Ridge, Weather or Hawk Eye. Hawk Eye provides autonomous flight and perches; **Theatre** supports landscape viewing with controls that hide while idle. Tap to reveal controls. Night visibility and comfort controls are under **More**.

This single-location testing build includes fixed scenery; address entry is not supported. Home details, inferred trees and reconstructed weather are approximations. Physical Pixel endurance testing and recorded-storm validation remain unfinished.

The APK's SHA-256 is listed in `SHA256SUMS.txt` and identifies the tested build.
