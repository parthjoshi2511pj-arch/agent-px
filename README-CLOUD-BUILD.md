# AGENT PX — Android cloud build starter

This archive contains the native Kotlin/Jetpack Compose Android project files extracted from the supplied AI Studio project, the AGENT PX logo, and a GitHub Actions workflow that builds a debug APK in the cloud.

## Build from an Android phone/tablet (no PC required)

1. Sign in to GitHub and create a new **private** repository named `AgentPX-Android`.
2. Upload the contents of this ZIP (extract it first using your device's file manager; upload the folders and files to the repository root).
3. Open the repository's **Actions** tab and allow workflows if GitHub asks.
4. Run **Build Agent PX APK** using **Run workflow** (or wait for the first push build).
5. When it finishes, open the run, scroll to **Artifacts**, and download `Agent-PX-debug-APK`.
6. Extract the artifact ZIP and install `app-debug.apk` on your Android device. Android may ask you to allow installs from that browser/file manager.

## Important status and limitations

- This is a **cloud-build starter project**, not an APK. The APK is created only after a successful GitHub Actions build.
- The Kotlin templates have not been compiled or device-tested in this environment. If the build reports errors, open the Actions run log and share the error text so the project can be corrected.
- Android only permits device operations that the OS exposes and the user explicitly authorizes. Accessibility, notification access, microphone, calls, SMS, and background microphone use have special restrictions. This app cannot have unrestricted control over every Android function.
- Gemini API credentials must not be hard-coded into the APK. Configure a secure backend before enabling real Gemini requests in production.
