# Change Log 📝

Chronological record of all updates, bug fixes, and refinements for **Japanese Music Station**.

---

## 📦 [Version 1.6.0] — Interactive Ambience (Time, Weather & Synthesized Audio) 🌌🌧️
*Release Date: August 27, 2026*

### 1. New Ambience Control System
* **Header Button Replacement**: Replaced the obsolete `SFX ON / OFF` button in the top-right header with a dedicated **`AMBIENCE`** button (Keyboard Shortcut: **`A`**).
* **Ambience Settings Modal**: Opens a retro arcade-styled pop-up with two distinct setting categories:
  * **1. TIME OF DAY**:
    * **`DAY`**: Vibrant daytime cyan/sky blue gradient, clear Mount Fuji silhouette, daytime building facade.
    * **`DUSK`**: Classic twilight purple/sunset orange sky with warm glowing windows and neon signage.
    * **`NIGHT`**: Deep starry midnight sky with illuminated Tokyo Tower and radiant neon signs.
  * **2. WEATHER & AMBIENCE**:
    * **`CLEAR`**: Pure clear sky with silent background (music only).
    * **`RAIN`**: Canvas-driven pixel rain droplet animation + continuous procedural rain sound synthesis via Web Audio API.
    * **`SNOW`**: Drifting pixel snowflakes animation + soft procedural wind/breeze audio synthesis via Web Audio API.

### 2. State & Audio Persistence
* Ambience selections (`TIME` and `WEATHER`) are automatically saved to `LocalStorage` and restored seamlessly upon page reload.
* Audio generators automatically synchronize with weather changes and stop cleanly when switching to `CLEAR` or unmounting.

---

## 📦 [Version 1.5.6] — Unobstructed Video Display & UI Symmetry 🛠️
*Release Date: August 26, 2026*

* Removed the floating `ON AIR` badge inside the 16:9 display that was covering YouTube's Settings Gear (⚙️).
* Symmetrized typography and framing between Queue and History sub-panels.
* Embedded SVG Favicon to eliminate 404 errors.

---

## 📦 [Version 1.5.5] — Symmetrical Panels & Favicon Integration 🎨
*Release Date: August 26, 2026*

* Standardized typography, colors, and layout symmetry between Queue and History sub-panels.

---

## 📦 [Version 1.5.4] — Universal CORS-Free YouTube Search Engine 🔍
*Release Date: August 26, 2026*

* Rebuilt search engine with multi-proxy fallback and direct YouTube HTML parser.

---

## 📦 [Version 1.5.3] — Unified Button System & Group Dimensions 📐
*Release Date: August 25, 2026*

* Standardized button color states (`[unclicked]` vs `[clicked]`) and group button sizing.

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
