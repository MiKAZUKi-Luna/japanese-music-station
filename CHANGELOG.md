# Change Log 📝

Chronological record of all updates, bug fixes, and refinements for **Japanese Music Station**.

---

## 📦 [Version 1.5.6] — Right Panel Height Optimization & Row Streamlining 📐
*Release Date: August 27, 2026*

### 1. 100% Vertical Space Utilization in Right Panel
* **Dynamic Full-Height Layout**: Replaced the fixed `max-h-[560px]` constraint with flexbox auto-stretching (`flex: 1 1 0%` + `min-height: 0`). The Queue and History scrollable lists now expand to occupy the entire vertical height of the panel, eliminating empty bottom gaps and fitting more songs comfortably.

### 2. Streamlined Single-Line Track Rows (Fixed Text Overlapping)
* **Removed Redundant Sub-Labels**: Removed `ID:` and `Added:` timestamps from both Queue and History rows.
* **Clean Single-Line Layout**: Track titles now occupy a single, crisp line with automatic text truncation (`...`), preventing text stacking or overlapping when resizing the browser window.

### 3. History-to-Queue Transfer Cleanup
* **Auto-Removal on Re-queue**: Clicking **`+ ADD TO QUEUE`** in the History tab now transfers the song into the active Queue and immediately removes it from History, avoiding redundant duplicate listings.

### 4. Unobstructed Video Display
* **Removed Floating 'ON AIR' Badge Overlay**: Removed the overlay badge from inside the 16:9 video frame that was obstructing YouTube's native Settings Gear (⚙️) and CC buttons.

---

## 📦 [Version 1.5.5] — Symmetrical Panels & Favicon Integration 🎨
*Release Date: August 27, 2026*

* Standardized typography, colors, and layout symmetry between Queue and History sub-panels.
* Embedded inline SVG pixel music note favicon (`♫`) in `<head>` to prevent `favicon.ico 404` errors.

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
