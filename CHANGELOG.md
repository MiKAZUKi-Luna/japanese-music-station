# Change Log 📝

Chronological record of all updates, bug fixes, and refinements for **Japanese Music Station**.

---

## 📦 [Version 1.5.3] — Unified Button System & Group Dimensions 📐
*Release Date: August 25, 2026*

### 1. Unified Button State Styling
* **Universal Color States**: Standardized all buttons across the app to share identical visual feedback:
  * **[Unclicked / Default]**: White text (`#FFFFFF`), dark purple background (`#2A2238`), and lighter contrast pixel border (`#3D2F4C`).
  * **[Clicked / Active]**: Dark text (`#131021`), bright neon pink background (`#F57D7C`), and gold contrast border (`#FFC061`).
* Eliminates inconsistent color mismatches across active tabs, transport modes, speed buttons, and utility toggles.

### 2. Group Button Sizing & Dimensions
* **Tabs**: `QUEUE` and `HISTORY` tabs are now perfectly symmetrical with equal 50/50 width and height (44px).
* **Transport Controls**: `Previous`, `Play/Pause`, and `Next` buttons share matching unified heights (46px).
* **Mode Toggles**: `Loop`, `Shuffle`, and `CC` share identical dimensions (40px height, 95px min-width).
* **Speed Selectors**: `0.75x`, `1x`, `1.25x`, and `1.5x` share matching dimensions (32px height, 54px width).
* **Form Action Buttons**: `ADD URL` and `SEARCH` share matching dimensions (44px height, 110px min-width).
* **Header Buttons**: `SFX` button sized to 38px height and 110px min-width (prepared for matching `AMBIENCE` button).

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
