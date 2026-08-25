# Change Log 📝

Chronological record of all updates, bug fixes, and refinements for **Japanese Music Station**.

---

## 📦 [Version 1.4.0] — Minimalist UI & Full English Localization
*Release Date: August 25, 2026*

### 1. Minimalist Display Area
* **Removed**: The large `80s` pixel art text and cassette emoji `📼` from the standby screen.
* **Removed**: Headphone, cat, and disc emojis (`🐱🎧 💽`) from the top-right overlay.
* **Refined**: Clean, modern typography with a sleek, minimalist `● ON AIR` live indicator.

### 2. Full English Localization
* Converted all UI text, tooltips, placeholders, button labels, and system notifications from Thai and Japanese into clean, concise English.
* Replaced background neon signage in the SVG landscape with retro English/Romaji signage (`MIDNIGHT`, `CITY POP`, `NIGHT FLIGHT BAR`, `CAFE 80s`).

### 3. Default Volume Adjustment
* Set initial default volume level to **25%** (was 80%) for a more comfortable first-listen experience.

---

## 📦 [Version 1.3.0] — Chronological History & Re-queue Fix
*Release Date: August 24, 2026*

### 1. Chronological History Numbering
* Updated history tracking to append sequentially so that the 1st song played is labeled **1.**, the 2nd song **2.**, and subsequent tracks follow natural chronological order.

### 2. Fixed "+ ADD TO QUEUE" in History
* Fixed missing prop connection on the History re-add button. Clicking `+ ADD TO QUEUE` now reliably re-queues the track with sound effects and a toast alert.

---

## 📦 [Version 1.2.0] — YouTube Native Controls & CC Support
*Release Date: August 24, 2026*

### 1. Enabled YouTube Native Controls (`controls: 1`)
* Enabled native player toolbar inside the 16:9 display, restoring the Settings Gear (⚙️) for video resolution (1080p/720p/4K) and the native CC subtitle button.

### 2. Dedicated CC Pixel Button
* Added a dedicated `CC` shortcut toggle button on the bottom retro transport bar.

---

## 📦 [Version 1.1.0] — Copyright Cleanup & Pure Queue Mode
*Release Date: August 24, 2026*

### 1. Removed Copyrighted Presets
* Removed the "+5 Recommended" button and pre-loaded sample songs that were subject to region blocks/takedowns.
* Removed the "Curated Library" tab and quick-select dropdown.
* Configured the queue to start cleanly at 0 tracks.

### 2. Independent Queue Workflow
* Adding a track via URL now cleanly appends to the queue without forcefully hijacking or auto-playing if the player is idle.

---

## 📦 [Version 1.0.0] — Initial Release
*Release Date: August 24, 2026*

* Single-file architecture with React 18, Babel Standalone, and Tailwind CSS CDN.
* 16/32-bit procedural SVG dusk cityscape background with Mt. Fuji, power lines, and CRT scanline filter.
* 65:35 responsive layout with YouTube IFrame API integration and 8-bit Web Audio SFX.
