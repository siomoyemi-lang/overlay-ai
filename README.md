# Overlay AI (FloatingAI)

An undetectable Android application that provides a floating AI bubble overlay using an Accessibility Service. 

## Features
* **Undetectable Operation (Main Feature):** Operates silently in the background reading screen context via accessibility nodes without triggering standard screen recording, screenshot, or visibility alerts.
* **Bring Your Own Key (BYOK):** Connect your preferred AI model by providing your own API key.
* **Floating Bubble Interface:** Persistent screen overlay for quick AI access (\FloatingAIService.kt\).
* **Settings Management:** Configurable preferences via \SettingsActivity.kt\.
* **Clipboard Handling:** Prevents auto-clipboard overwriting on bubble expansion.

## Supported AI Providers
You must provide your own API key for the AI context generation to function. The app currently supports:
* OpenAI
* Google Gemini
* Anthropic (Claude)

### How to Add Your API Key
1. Open the **Overlay AI** app on your device.
2. Navigate to the **Settings** menu.
3. Select your preferred AI Provider.
4. Paste your secret API key into the input field and save. 
*(Note: Your API key is stored locally on your device and is never shared).*

## Getting Started
1. Clone this repository.
2. Open the project in **Android Studio**.
3. Sync the Gradle files.
4. Build and run the app on an Android device or emulator.

## Permissions Setup (Required)
For the floating bubble and AI context to function, you must manually grant two system permissions.

**1. Grant "Display Over Other Apps"**
* Go to your device **Settings** > **Apps** > **Special app access**.
* Tap on **Display over other apps** (or "Draw over other apps").
* Find and select **Overlay AI**.
* Toggle **Allow display over other apps** to **ON**.

**2. Grant "Accessibility" Access**
* Go to **Settings** > **Accessibility**.
* Look under **Downloaded apps** (or **Installed apps**) and tap **Overlay AI**.
* Toggle the service to **ON**.

> **Note for Android 13+:** If the Accessibility setting is greyed out with a "Restricted setting" warning (which happens automatically for sideloaded/development apps):
> 1. Go to **Settings** > **Apps** > **See all apps** > **Overlay AI**.
> 2. Tap the three dots (**⋮**) in the top right corner of the app info screen.
> 3. Tap **Allow restricted settings**.
> 4. Authenticate if prompted, then go back to the Accessibility menu to toggle the service ON.
