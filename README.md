# Japanese Music Station (v1.5.3) 🎵🌆

A retro-futuristic YouTube music queue player with a **Pixel Art × 80s City Pop** aesthetic. Built as a single self-contained HTML file that runs instantly by double-clicking or can be deployed directly to Netlify via GitHub with zero build steps or npm installations.

---

## 🕹️ 1. Key Highlights & Features

* **Unified Retro Button System**: Strict, consistent button states across the entire application — unclicked (white text, dark base, border) and clicked (dark text, bright pink/gold base, contrast border).
* **Proportional Group Sizing**: Buttons in the same functional groups (Tabs, Transport, Modes, Speeds, Actions, Header) share matching heights, widths, and alignments.
* **Dedicated Arcade Music Search**: Search YouTube music in real-time with 1-click **`+ ADD QUEUE`** or **`PLAY`** actions using the dedicated **`SEARCH`** button or keyboard shortcuts (**`/`** and **`Ctrl + K`**).
* **Virtual 80s DJ Booth**: Inspired by retro pixel art environments and Japanese City Pop vibes.
* **16/32-Bit Procedural Dusk Cityscape**: Features Mount Fuji, Tokyo Tower, overhead power lines, and glowing retro neon signs.
* **Full YouTube Native Controls**: Settings Gear (⚙️) for 1080p/720p resolution and CC Subtitle toggle without Player Error 153.
* **Smart Queue & History**: Re-order, delete, clear, and re-add previously played tracks in chronological order.

---

## 🎨 2. Color Palette & Styling Constraints

### Color Palette (Exact Hex)
* **Sky top (navy)**: `#1F1A3A`
* **Sky mid (purple)**: `#5B3256`
* **Sky sunset**: `#A2536A`
* **Sky dusk (orange)**: `#E08573`
* **Building shadow**: `#131021`
* **Wall base**: `#2A2238`
* **Warm light accent**: `#FFC061`
* **Neon pink accent**: `#F57D7C`
* **Panel background**: `#1D1728` (90% opacity)
* **Pixel border**: `#3D2F4C`

### Strict Pixel Rules
* **Zero Border-Radius**: 100% hard-edged pixel styling.
* **Pixel Borders & Shadows**: 2–4px solid `#3D2F4C` with `4px 4px 0px #000` drop-shadows that depress on click (`translate(2px, 2px)`).
* **Typography**: Google Fonts `Press Start 2P` for headers, `VT323` for body text, and `Silkscreen` for sub-labels.
* **Step Transitions**: Retro `steps()` animation curves for authentic vintage responsiveness.

---

## 📐 3. Layout & Architecture (65% : 35% Grid)

### Left Panel (65% — Player & Controls):
1. **16:9 YouTube Screen**: YouTube IFrame Player with full native controls (Settings Gear ⚙️ and CC button), custom pixel visualizer equalizer, and a minimalist on-air status badge.
2. **Now Playing Info Bar**: Scrolling marquee title, Video ID, time elapsed/total, and an interactive pixel scrubber bar.
3. **URL Input & Arcade Search**: Paste any YouTube link and click **ADD URL**, or click **SEARCH** to open the Arcade Search modal.
4. **Transport Controls**:
   * ⏮ Prev (Restart / Previous track)
   * ⏯ Play / Pause
   * ⏭ Next (Skip to next track)
   * Loop Mode (Off / Loop 1 / Loop All)
   * Shuffle Queue
   * CC Subtitles Toggle
   * Speed Selectors (0.75x, 1x, 1.25x, 1.5x)
   * Volume Slider (Default: 25%) & Mute Button
   * Clear Queue

### Right Panel (35% — Queue & History):
1. **QUEUE Tab**: Manage queued tracks with [PLAY], [▲] Move Up, [▼] Move Down, and [✕] Delete actions, plus "CLEAR ALL QUEUE".
2. **HISTORY Tab**: Tracks played in chronological order (1., 2., 3...) with a 1-click **`+ ADD TO QUEUE`** button.

---

## 🛠️ 4. Tech Stack

* **HTML5 / Single File**: Entire application in `index.html` (or `japanese-music-station-v1.5.3.html`) with zero dependencies.
* **React 18 & Babel Standalone**: Client-side reactive UI via Cloudflare CDNjs.
* **Tailwind CSS**: Utility styling with inline configuration.
* **YouTube IFrame API**: Video playback and state synchronization.
* **Web Audio API**: Real-time 8-bit retro sound synthesizer (SFX).
* **LocalStorage**: Persistent queue, history, and volume settings.
