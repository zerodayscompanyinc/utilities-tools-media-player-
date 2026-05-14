 

***

# ZeroDays Media Player

A modern, cyber-themed media player built with pure HTML, CSS, and JavaScript.  
Supports audio, video, YouTube, Spotify, and SoundCloud playback. Features a local encrypted account system, playlist management, quick-access sessions, drag-and-drop file support, and PWA capabilities.

---

## 🌐 Live Site

### HTTPS
- [ZeroDays Media Player (Secure)](https://media-player-no-ads.vercel.app/?utm_source=chatgpt.com)

### HTTP
- [ZeroDays Media Player (HTTP)](http://media-player.ultimatetool.2bd.net/?utm_source=chatgpt.com)

---

# ✨ Features

## 🎵 Media Playback & Universal Support
- **Audio & Video**: Native playback for MP3, MP4, WebM, OGG, WAV, FLAC, M4A, AAC, MKV, AVI.
- **YouTube Integration**: Automatically converts standard YouTube links to embeddable iframes.
- **oEmbed Platform Support**: Automatically fetches and embeds players for:
  - **Spotify** (Tracks/Playlists) - reviews song only no full songs
  - **SoundCloud**
  - **Mixcloud**
  - **Deezer**
  - **Apple Music**
- **Local Files**: Drag & drop or select local audio/video files for instant playback.
- **Visualizer**: Real-time Canvas-based audio spectrum visualizer with dynamic color bars.

## 🎛️ Playback Controls
- Play / Pause / Next / Previous
- Volume Control with Slider
- Repeat Mode Toggle (Off/On)
- Track Filtering: All, Audio, Video, Favorites.
- Searchable Playlist
- Shuffle Playlist
- Remove individual tracks or clear all.

## 👤 Local Account System
- **Encrypted Storage**: User data is stored locally using a custom XOR-based encryption layer.
- **Authentication**:
  - **Standard**: Register/Login using Email and Password.
  - **Quick Access**: Instant session creation using any username (no password required).
  - **Password Reset**: Local password reset functionality via email verification.
- **Session Persistence**: User sessions and playlists remain active after closing the browser.
- **Multi-user Support**: Each user (email or quick-access) has their own isolated playlist.

## ⌨️ Keyboard Shortcuts
- `Space`: Play / Pause
- `→`: Next Track
- `←`: Previous Track
- `↑`: Volume Up
- `↓`: Volume Down
- `R`: Toggle Repeat
- `F`: Toggle Favorite (Current Track)
- `ESC`: Close Shortcut Overlay

## 📱 Progressive Web App (PWA)
- Installable on supported browsers and mobile devices.
- App-like interface with "Install App" button.
- Optimized for standalone mobile usage.

---

# 🛠️ Built With

- **HTML5**: Semantic structure and Media elements.
- **CSS3**: Flexbox/Grid layouts, Glassmorphism, Cyber-aesthetic styling, Animations.
- **JavaScript (Vanilla)**:
  - Web Audio API (for the visualizer).
  - Canvas API (for rendering).
  - LocalStorage API (for data persistence).
  - Fetch API (for oEmbed data).
  - File API (for local file handling).
  - Crypto (custom XOR obfuscation).

---

# 📦 Supported Media Types

| Type | Format/Platform | Support Status |
|------|-----------------|----------------|
| **Audio** | MP3, WAV, OGG, FLAC, M4A, AAC | ✅ Native |
| **Video** | MP4, WebM, MKV, AVI, MOV | ✅ Native |
| **Streaming** | YouTube | ✅ Iframe Embed |
| **Streaming** | Spotify | ✅ oEmbed Integration |
| **Streaming** | SoundCloud | ✅ oEmbed Integration |
| **Streaming** | Deezer, Mixcloud | ✅ oEmbed Integration |
| **Local Files** | Drag & Drop / File Select | ✅ Blob URL |

---

# 🚀 Installation & Usage

## Local Usage
1. Download the source code (single `index.html` file recommended).
2. Open `index.html` in any modern web browser.
3. Allow permission for Audio Context if prompted (for the visualizer).

## PWA Installation
1. Open the **HTTPS** version of the site.
2. Click the **📱 INSTALL APP** button in the header.
3. Follow the browser prompt to add to your home screen.

---

# 🔐 Security & Storage Architecture

## Data Privacy
- **Local-Only**: All data (playlists, user credentials) is stored in the user's browser `localStorage`.
- **No Server**: No data is sent to external servers (except for fetching public oEmbed data from Spotify/SoundCloud).
- **Encryption**: User database is obfuscated using a Base64 + XOR cipher before storage.

## Account Sync
- Playlists are automatically synced to the currently logged-in user's profile.
- "Guest" mode uses a local generic playlist if no user is logged in.

---

# ⚠️ Notes

- **CORS & Embeds**: Some streaming platforms (like Spotify) may restrict playback based on geographical location or browser embedding policies.
- **Local Files**: Local file URLs (`blob:`) are temporary and will be lost if the page is refreshed completely (re-adding files is required).
- **iOS PWA**: Visualizer and autoplay features may behave differently on iOS due to system restrictions.

---

# 📄 License

This project is for educational and personal use.

---

# 🖤 ZeroDays Project

> ZERO DAYS • MEDIA PLAYER • GLOBAL ACCOUNT ACCESS • QUICK LOCAL SYNC • NO API KEYS
