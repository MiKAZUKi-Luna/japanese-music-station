# Change Log 📝

Chronological record of all updates, bug fixes, and refinements for **Japanese Music Station**.

---

## 📦 [Version 1.5.4] — Universal CORS-Free YouTube Search Engine 🔍
*Release Date: August 26, 2026*

### 1. Fixed CORS Block on YouTube Search
* **Problem**: Invidious API instances blocked cross-origin requests from `*.netlify.app` with CORS 403 / 401 errors, leaving the search modal in an endless loading state.
* **Solution**: Rebuilt the search engine with a **Multi-Tier CORS-Free Architecture**:
  * **Tier 1 (Official YouTube Parser)**: Scrapes and parses official `ytInitialData` directly via reliable CORS proxies, returning live YouTube search results.
  * **Tier 2 (Piped API Fallback)**: Multi-instance Piped API endpoints configured with `Access-Control-Allow-Origin: *`.
  * **Tier 3 (Proxied Invidious)**: Invidious API piped through CORS proxies.
  * **Tier 4 (Direct URL / ID Parser)**: Instant recognition and parsing when a direct YouTube link is entered into the search bar.

---

## 📦 [Version 1.5.3] — Unified Button System & Group Dimensions 📐
*Release Date: August 25, 2026*

* Standardized all button states across the app (`[unclicked]` vs `[clicked]`).
* Harmonized dimensions across button groups (Tabs, Transport, Modes, Speeds, Form actions).

---

## 📦 [Version 1.5.2] — CRT Removal & Search Modal Decluttering 🧹
*Release Date: August 25, 2026*

* Removed `CRT ON / OFF` button and scanline layer.
* Removed `TRENDING:` suggestion tags from the Arcade Search modal.

---

## 📦 [Version 1.5.1] — UI Decluttering & Layout Hardening 🛠️
*Release Date: August 25, 2026*

* Streamlined search triggers into a single dedicated `SEARCH` button beside `ADD URL`.
* Replaced the letter `J` in the header with a pixel music note icon (`♫`).
* Fixed YouTube Error 153 and hardened the 65:35 responsive layout with standalone CSS.

---

## 📦 [Version 1.5.0] — Arcade Style Search Pop-up Modal 🕹️
*Release Date: August 25, 2026*

* Added a retro arcade-themed search pop-up window (`ArcadeSearchModal`) for real-time YouTube music discovery without copy-pasting URLs.

---

## 📦 [Version 1.4.0] — Minimalist UI & Full English Localization
*Release Date: August 25, 2026*

* Removed large `80s` pixel text and emojis (`📼`, `🐱🎧 💽`).
* Converted all UI text into English and set default volume to 25%.

---

## 📦 [Version 1.3.0] — Chronological History & Re-queue Fix
*Release Date: August 24, 2026*

* Changed history tracking to chronological order (1st song = 1., 2nd song = 2.).
* Fixed prop wiring for `+ ADD TO QUEUE` in the History tab.

---

## 📦 [Version 1.2.0] — YouTube Native Controls & CC Support
*Release Date: August 24, 2026*

* Enabled YouTube Native Controls (`controls: 1`) to restore the Settings Gear (⚙️) and CC subtitle button.

---

## 📦 [Version 1.1.0] — Copyright Cleanup & Pure Queue Mode
*Release Date: August 24, 2026*

* Removed copyrighted demo tracks and configured queue to start cleanly at 0 tracks.

---

## 📦 [Version 1.0.0] — Initial Release
*Release Date: August 24, 2026*

* Single-file architecture with React 18, Babel Standalone, and Tailwind CSS CDN.
* 16/32-bit procedural SVG dusk cityscape background with Mt. Fuji, power lines, and 65:35 responsive layout.
