# Change Log 📝

Chronological record of all updates, bug fixes, and refinements for **Japanese Music Station**.

---

## 📦 [Version 1.5.5] — Unobstructed Video Display, Panel Symmetry & Favicon 🛠️
*Release Date: August 27, 2026*

### 1. Unobstructed 16:9 Video Screen
* **Removed Floating 'ON AIR' Badge Overlay**: Removed the small rectangular overlay badge inside the top-right corner of the video area that was obstructing YouTube's native Settings Gear (⚙️) and Share controls. The top status indicator (`● ON AIR` / `■ STANDBY`) in the booth frame header remains intact.

### 2. Symmetrical Typography & Layout for Right Panel
* **Empty State Cards**: Harmonized font families (`Press Start 2P` header, `VT323` subtitle), colors (`#FFC061` header, `#E08573` subtitle), and box sizes across both `QUEUE` and `HISTORY` tabs.
* **Track Rows & Action Bars**: Aligned row item fonts (`VT323 text-lg`), index badges (`#E08573`), button heights (`28px`), and footer Clear buttons (`36px`).

### 3. Integrated SVG Favicon (Fixed Favicon 404)
* Embedded an inline SVG music note favicon (`♫`) in the HTML `<head>` data URI to prevent browser 404 errors for `favicon.ico`.

---

## 📦 [Version 1.5.4] — Universal CORS-Free YouTube Search Engine 🔍
*Release Date: August 26, 2026*

* **Fixed CORS Block on Search**: Rebuilt the search engine with a multi-proxy fallback and direct YouTube HTML parser, ensuring reliable search results across all browsers without API keys.

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
