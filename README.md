# ✦ AEROGRAM — APK Releases

> **Connect Beyond Boundaries**

Download the latest AEROGRAM APK builds here.

## 📥 Latest Release

| Version | Type | Download |
|---------|------|----------|
| **v7.0.0** | Debug | [aerogram-v7.0.0.apk](releases/v7.0.0/aerogram-v7.0.0.apk) |
| v6.0.0 | Debug | [aerogram-v6.0.0.apk](releases/v6.0.0/aerogram-v6.0.0.apk) |
| v5.2.0 | Debug | [aerogram-v5.2.0.apk](releases/v5.2.0/aerogram-v5.2.0.apk) |
| v5.0.0 | Debug | [aerogram-v5.0.0-debug.apk](releases/v5.0.0/aerogram-v5.0.0-debug.apk) |
| v4.0.0 | Debug | [aerogram-v4.0.0-debug.apk](releases/v4.0.0/aerogram-v4.0.0-debug.apk) |
| v3.0.0 | Debug | [aerogram-v3.0.0-debug.apk](releases/v3.0.0/aerogram-v3.0.0-debug.apk) |
| v2.0.0 | Debug | [aerogram-v2.0.0-debug.apk](releases/v2.0.0/aerogram-v2.0.0-debug.apk) |
| v1.1.0 | Debug | [aerogram-v1.1.0-debug.apk](releases/v1.1.0/aerogram-v1.1.0-debug.apk) |
| v1.0.0 | Debug | [aerogram-v1.0.0-debug.apk](releases/v1.0.0/aerogram-v1.0.0-debug.apk) |

## 📝 Changelog

### v7.0.0 — Notification Center, Database v4 Upgrade & Home Header Integration
- 🔔 **Notification Center** — Introduced a full-screen Notification Center to view system updates, new follower alerts, messages, and likes.
- 💬 **Home Header Integration** — Integrated a styling-matched notification bell icon in the Chats list header with a dynamic red unread dot badge.
- 🗄️ **Database v4 Upgrade** — Created `aero_notification` SQLite table and seeded initial system, follower, and post like notifications.
- ⚙️ **Actions & Controls** — Implemented marking notifications as read by tapping, bulk "Mark all as read" actions, and clearing notifications history.

### v6.0.0 — Chat Creation Screen, Message Actions & Reels Removal
- ✏️ **Chat & Group Creation** — Added full-screen page for starting chats, creating groups, and creating channels via a routing flow instead of popups.
- 👤 **Followers & Following Selectors** — Easily add followers, following, or random public accounts directly to groups or channels.
- 🗑️ **Reels Removal** — Completely removed the Reels page and button, leaving a clean discovery-focused Explore page.
- 💬 **Message Actions** — Implemented deleting messages, deleting whole chats, editing messages, and forwarding/saving messages.
- 🗄️ **Saved Messages** — Created a dedicated "Saved Messages" chat repository for personal text/media storage.

### v5.2.0 — Dedicated Edit Profile Page & Privacy Control Enforcement
- 👤 **Dedicated Edit Profile Screen** — Replaced the pop-up profile editor dialog with a dedicated, beautiful full-screen profile editor.
- 🔒 **Privacy Switch** — Added a dedicated switch to toggle profile privacy (Public vs. Private) with detailed descriptions explaining their rules.
- 🕵️ **Search Visibility Enforcement** — Private profiles are completely hidden from user lists, popular creators carousels, and universal search results (reels, statuses, profiles).
- 🚫 **Chat Initiation Restricting** — Disallowed starting direct chats with private profiles from the contacts directory.
- 🛡️ **Message Blocking** — Added warning banner and disabled message inputs in direct chats with private accounts unless they message you first.
- 🧹 **Cleanups & Version Bump** — Consolidated Profile screen, removed duplicate settings items, and updated build target to v5.2.0.

### v5.0.0 — Explore Page & Full Settings Panel
- 🔍 **Explore Page** — Replaced the Status tab with a full-featured Explore page featuring search bar, filter chips (All/Users/Hashtags/Posts), and discovery feed.
- 🏷️ **Trending Hashtags** — Auto-parsed hashtags from reels and statuses displayed as horizontally scrollable trending cards.
- 👥 **Popular Creators** — Discover users with follower counts in a horizontal carousel with avatar cards.
- 🎬 **Explore Discoveries Grid** — 2-column gradient reel grid with preview dialogs showing likes, comments, and full reel details.
- 🔎 **Universal Search** — Search across usernames, bios, hashtags, reel descriptions, and status captions with categorized results.
- 🛠️ **Full Settings Panel** — Replaced popup settings dialog with a dedicated full-screen settings panel organized into categories.
- 🔐 **Hardware Keystore Indicator** — Settings panel shows AES-GCM encryption status for the seed phrase.
- 🧹 **Compilation Fix** — Resolved missing `User` model import in ProfileScreen for clean builds.

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
