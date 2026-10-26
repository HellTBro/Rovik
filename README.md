# Rovik — Studio Music Desktop Player

A modern, high-fidelity minimalist music player built for desktop platforms with Electron, React, TypeScript, and Vite, powered by Supabase.

Official Channel: [YouTube (@Hell_BroX)](https://www.youtube.com/@Hell_BroX)

---

## Architecture and Core Capabilities

### 1. Audio Engine and Processing
- 32-bit Float DSP Audio Pipeline with Web Audio API.
- 10-Band Graphic Equalizer with studio presets and custom frequency shaping.
- Real-time Studio Spectrum Analyzer with FFT-based responsive frequency visualization.
- Pitch-preserving variable playback speed (0.5x – 2.0x).
- Playback queue with reordering, shuffle, repeat-queue, and single-track loop modes.
- Hardware media keys and Windows MediaSession integration.

### 2. Lyrics Canvas and Karaoke
- Fullscreen Canvas with synchronized LRC lyrics.
- Dual-Mode Lyrics Animation:
  - Letter Flow: Smooth progressive letter-by-letter vocal fill with dual-line preview.
  - Alternating Focus: Dynamic active line illumination with cinematic focus switching.
  - Custom Atmospheric Glow and subtle dynamic typography.

### 3. Music Catalog and Offline Vault
- Unified catalog integrating Rovik Studio releases, Audius decentralized tracks, and YouTube Music streams.
- Offline Vault ("My Music"): Complete local playback with IndexedDB caching and direct disk import (.mp3, .flac, .wav, .ogg, .m4a).
- Non-blocking top-left download manager with concurrent download queuing and live progress tracking.
- Fast local and remote search across millions of tracks.

### 4. Interface and Customization
- Refined frosted glass design with dark studio palette.
- Dynamic background engine supporting custom images, video wallpapers, or artist banners.
- Granular control over background dimming, blur, surface transparency, and corner curvature.
- Strict absence of neon artifacts and cluttered borders.
- Bilingual interface (Russian and English).

### 5. Cloud Profiles and Metrics
- Supabase authentication with persistent sessions and security.
- Cloud synchronization for liked tracks, collaborative playlists, and user profiles.
- Precise listening analytics: total listening hours, track counts, and real-time play incrementation.

---

## Quick Start

### Development Environment

1. Clone repository and navigate to desktop workspace:
```bash
cd apps/desktop
```

2. Install dependencies:
```bash
npm install
```

3. Start Vite development server:
```bash
npm run dev
```

4. Launch Electron window:
```bash
npm start
```

### Production Build

To build the standalone Windows installer (NSIS):
```bash
npm run dist
```
The output installer will be generated in:
`apps/desktop/dist-release/Rovik Setup 1.0.0.exe`

---

## Links and Resources

- YouTube: https://www.youtube.com/@Hell_BroX
- License: Rovik Ethical & Creative Public License (NECPL v1.0)
