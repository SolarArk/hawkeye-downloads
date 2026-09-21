# Hawk Eye 0.2.1 test build

Version 0.2.1, Android version code 3. Install over the existing Hawk Eye app to preserve settings. Requires Android 8.0/API 26 or newer and OpenGL ES 3.0.

- Automatic hosted HTTPS weather updates with source freshness, retry, cached startup and conditional requests. The built-in service requires no key or activation step; its internal credential remains on the server.
- Readable nighttime lighting, collapsible weather details and a compact Views/Layers/More dock.
- Yard view, autonomous Hawk Eye flight, tree and home perches, and landscape Theatre controls.
- Nested terrain detail, an estimated gambrel home roof, entrance and patio, and canopy-aware flight clearance.
- Spatial rain, observed regional lightning illumination, bounded weather reconstruction and comfort controls.
- Bounded terrain loading and adaptive render resolution, rain density and frame targets.

The APK retains the existing development signing identity. Version 0.2.1 passed 52 Android tests, Android lint with zero errors/22 existing warnings, 113 package integrity checks, and emulator signed-update/fresh-settings checks with no saved weather key. The Worker passed 17 tests and a deployment dry run. After deployment, the app showed Live weather with an empty saved key, six successful sources and no crash. Hosted checks verified public weather, protected health access and conditional updates.

The preceding rendering and terrain-queue implementation passed a 183-second emulator soak without an out-of-memory failure. Version 0.2.1 changes connection guidance and server access, with no rendering changes.

The emulator checks do not certify sustained Pixel performance. Physical Pixel endurance tests, recorded-storm replay and forced hosted-cache recovery remain unvalidated. Terrain and structures contain estimates; weather is reconstructed from regional observations and model data, not measured at every rendered point. The maximum supported extrapolation interval remains 15 minutes, with source timestamps preserved.

The exact release checksum is in `SHA256SUMS.txt`.
