# Overlay AI (FloatingAI)

An Android application that provides a floating AI bubble overlay using an Accessibility Service. 

## Features
* **Floating Bubble Interface:** Persistent screen overlay for quick AI access (\FloatingAIService.kt\).
* **Accessibility Integration:** Uses Android Accessibility Services to interact with on-screen context.
* **Settings Management:** Configurable preferences via \SettingsActivity.kt\.
* **Clipboard Handling:** Prevents auto-clipboard overwriting on bubble expansion.

## Tech Stack
* Android / Kotlin
* Gradle

## Getting Started
1. Clone this repository.
2. Open the project in **Android Studio**.
3. Sync the Gradle files.
4. Build and run the app on an Android device or emulator.
5. **Note:** You will need to manually grant the app "Display over other apps" and "Accessibility" permissions in your device settings for the floating bubble to function correctly.
