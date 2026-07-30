# SafetyKit — distribution

Public download point for the **SafetyKit Kids** and **SafetyKit Parent**
Android apps. The application source lives in a separate, private repository;
only the installable builds and the version manifest are published here.

- `app-version.json` — the latest published build of each app. Both apps read
  this to decide whether to offer an in-app update.
- Releases — the APKs themselves, as assets named `safetykit-kids.apk` and
  `safetykit-parent.apk`.

These addresses are deliberately independent of the backend. The backend URL is
baked into each app at build time, so if the backend ever moves, an app that
could only ask the backend would never learn about the build that fixes it.
