# ✦ AEROGRAM — APK Releases

> **Connect Beyond Boundaries**

Download the latest AEROGRAM APK builds here.

## 📥 Latest Release

| Version | Type | Download |
|---------|------|----------|
| **v5.0.0** | Debug | [aerogram-v5.0.0-debug.apk](releases/v5.0.0/aerogram-v5.0.0-debug.apk) |
| v4.0.0 | Debug | [aerogram-v4.0.0-debug.apk](releases/v4.0.0/aerogram-v4.0.0-debug.apk) |
| v3.0.0 | Debug | [aerogram-v3.0.0-debug.apk](releases/v3.0.0/aerogram-v3.0.0-debug.apk) |
| v2.0.0 | Debug | [aerogram-v2.0.0-debug.apk](releases/v2.0.0/aerogram-v2.0.0-debug.apk) |
| v1.1.0 | Debug | [aerogram-v1.1.0-debug.apk](releases/v1.1.0/aerogram-v1.1.0-debug.apk) |
| v1.0.0 | Debug | [aerogram-v1.0.0-debug.apk](releases/v1.0.0/aerogram-v1.0.0-debug.apk) |

## 📝 Changelog

### v5.0.0 — Full Settings Panel & Polish
- 🛠️ **Full Settings Panel** — Replaced popup settings dialog with a dedicated full-screen settings panel organized into categories: Preferences, Security & Privacy, Profile & Customization, and Support.
- 🔐 **Hardware Keystore Indicator** — Settings panel shows AES-GCM encryption status for the seed phrase with a locked toggle.
- 🌐 **Inline Privacy Toggle** — Public/Private profile visibility can be toggled directly from the Settings panel's Security section.
- ✏️ **Edit Profile Access** — Quick-access link to the Edit Profile dialog from within Settings.
- 🧹 **Compilation Fix** — Resolved missing `User` model import in ProfileScreen for clean builds.
- 📐 **Category Headers** — Settings are organized with teal-colored category headers for clear visual grouping.

### v4.0.0 — Profile Customization & Settings Sync
- 👥 **Followers & Following Counters** — Mapped real-time social metrics directly from the SQLite database to the profile card.
- 🔒 **Public/Private Profile Visibility** — Added a glowing globe/lock badge that represents the user's privacy status in real-time.
- ⚙️ **Interactive Edit Profile Dialog** — Users can modify their Name, Bio, Avatar Initial letter, and gradient theme color index, instantly updating the local database.
- 🎛️ **App Settings Dialog** — Custom switches to toggle Notifications and Online Status visibility.
- 🔄 **StateFlow Syncing** — Reactive updates propagate database profile mutations to the main screen components instantly.

### v3.0.0 — Security & Version Upgrades
- 🔒 **Android Keystore AES-GCM Encrypted Security** — Added device-specific hardware-backed master key encryption to secure SQLite seed phrase data.
- 🛡️ **Hack-Proof Storage** — Prevented local plain-text private credential writing.
- 🛠️ **Tag Alignment** — Upgraded releases and Git tag structure to v3.0.0.

### v2.0.0 — SQLite Reactive Storage & Wallet Onboarding
- 🔐 **Seed Phrase Onboarding** — Integrated wallet-style 12-word seed phrase generation, copying, and validation.
- 📦 **Local SQLite Database** — Persists chats, message histories, status updates, and reels dynamically in SQLite (tables prefixed with `aero_`).
- 🔄 **Reactive UI State Flow** — Integrated Kotlin StateFlows in all screens for real-time updates upon sending messages, posting status updates, or liking reels.
- 💬 **Contacts Selector Dialog** — Added contacts selector dialog to start new conversations from seeded contacts.
- 👤 **Backup Seed Phrase** — Secure seed phrase viewing dialog inside settings.

### v1.0.0 — Initial Release
- 💬 **Chats** — Chat list with search, glassmorphic cards, message bubbles
- 🎬 **Reels** — Vertical pager short-video feed (YouTube Shorts style)
- 📱 **Status** — Story circles with gradient rings, full-screen viewer
- 👤 **Profile** — Profile card with stats, settings stubs
- 🎨 **Obsidian Couture Theme** — Dark glassmorphism with electric teal & amber accents
- 🔐 **Auth** — Login/Signup screens routed

## ⚙️ Installation

1. Download the APK file
2. Enable "Install from Unknown Sources" in your Android settings
3. Open the APK to install
4. Requires Android 7.0 (API 24) or higher

---

*Built with ❤️ using Kotlin + Jetpack Compose*
