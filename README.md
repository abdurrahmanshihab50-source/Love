# 💕 Reasons I Love You — 3D Romantic Keepsake Book

<p align="center">
  <img src="https://img.shields.io/badge/Experience-3D%20Interactive%20Book-ff4081?style=for-the-badge" alt="3D Experience">
  <img src="https://img.shields.io/badge/Audio-Web%20Audio%20Synthesizer-ffd700?style=for-the-badge" alt="Web Audio API">
  <img src="https://img.shields.io/badge/Atmosphere-Canvas%20Particles-7b1fa2?style=for-the-badge" alt="Canvas 2D Engine">
  <img src="https://img.shields.io/badge/Instagram-@the.cipher.stack-E1306C?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
</p>

---

## 📖 Overview

**Reasons I Love You** is a hyper-realistic 3D romantic keepsake book crafted in Vanilla HTML5, CSS3, and JavaScript. Designed with meticulous attention to typography, tactile physics, atmospheric lighting, and audio synthesis, it delivers an unforgettable interactive journey across 12 heartfelt chapters.

The experience starts with a closed, leather-bound, gold-filigreed 3D hardcover tome resting in gentle candlelight. Upon opening, the front cover swings open in 3D to reveal a two-page spread: a left-hand memory keepsake polaroid and a right-hand stack of 12 deckled page leaves that turn with realistic paper curling physics. After exploring all 12 reasons and secret love notes, the book gracefully closes in 3D with a grand celebratory confetti explosion and harmonic harp crescendo.

---

## ✨ Key Features

### 📕 1. Hyper-Realistic 3D Book Architecture
- **6-Faced Solid 3D Box Geometry**: Mathematically aligned front cover, raised ribbed leather spine, deckled cream pages edge, top, bottom, and back cover.
- **Antique Leather & Gold Filigree**: Rich burgundy leather texture, gold-foil corner brackets, and subtle candlelight specular glints.
- **Cinematic 3D Opening & Closing**: The cover physically swings open around the spine hinge (`rotateY(0deg) ➔ rotateY(-90deg)`), and seamlessly closes back upon completing the 12th page.

### 🔄 2. Physical 3D Page Leaf Turning
- **Spine Pivot Turning**: Page leaves rotate with realistic 3D perspective (`transform-origin: left center`) and dynamic curve shadows (`.is-turning`, `rotateY(-180deg)`).
- **Dual-Sided Page Content**:
  - **Front Face**: Heartfelt Reason, decorative quote marks, thematic SVG emblem, and interactive navigation hint.
  - **Back Face**: Hidden **"Secret Love Note"** revealed on the left side of the spread once turned.
- **Dynamic Polaroid Memories (Left Page)**: Synchronizes chapter title, handwritten quote, and atmospheric sky art to match each reason's theme.

### 🔒 3. 12th Page Automatic & Interactive Closing
- When reaching the 12th and final reason, the navigation button dynamically transforms into an animated glowing **"Close Book 📕"** control.
- Any forward action on the final page (clicking **Next / Close**, clicking **Leaf 12**, pressing <kbd>Space</kbd>, <kbd>→</kbd>, <kbd>Enter</kbd>, or swiping) triggers the full 3D closing animation.
- Triggers a grand multi-color rose petal and gold confetti shower with a musical harp crescendo, followed by a **"🌹 Read Again from the Beginning ✨"** replay CTA.

### 🎶 4. Web Audio API Music Box & SFX
- **Pure JavaScript Synthesizer**: Zero external audio files required. Uses standard `AudioContext`, dual sine/triangle oscillators, and exponential gain ramps.
- **Romantic Music Box Melody**: Plays a custom 15-note looped lullaby in the background.
- **Physical Paper Friction & Leather Thuds**: Bandpass-filtered white noise and low-frequency resonance simulate the tactile sound of turning pages and closing hardcover books.

### 🌌 5. Triple-Canvas Atmosphere Engine
1. **Ambient Background Canvas**: Twinkling stars, floating bokeh orbs, and drifting organic rose petals.
2. **Interactive Cursor Trail**: Generates golden stardust and shimmering sparkles on mouse/touch movement.
3. **Grand Finale Confetti**: Fullscreen explosion of rectangular foil and heart-shaped confetti on book closure.
4. **Flickering Candlelight Overlay**: Dynamic radial lighting with subtle organic scale and position sway.

### 💌 6. Real-Time Customizer Modal
- Personalize all 12 reasons and secret love notes on the fly.
- Add new custom reasons or delete existing ones.
- Automatically saves and restores customizations via browser `localStorage`.
- One-click restore to original romantic defaults.

---

## 🎮 Interaction & Controls

| Input | Action |
|---|---|
| **Click / Tap "Open the Book"** | Swings the 3D book open into reading mode |
| **Click Page / <kbd>→</kbd> / <kbd>Space</kbd>** | Turn to next page (or close book on page 12) |
| **<kbd>←</kbd> (Left Arrow)** | Turn back to previous page |
| **<kbd>Enter</kbd>** | Open book from intro / Close book on page 12 |
| **<kbd>M</kbd> / Music Button** | Toggle ambient music box soundtrack |
| **<kbd>R</kbd> (Reset)** | Restart and read again from the beginning |
| **Mobile Swipe Left / Right** | Turn page forward / backward with haptic vibration |
| **"Edit" Button** | Open customizer to edit reasons and love notes |
| **Instagram Icon** | Visit creator profile [`@the.cipher.stack`](https://instagram.com/the.cipher.stack) |

---

## 🛠️ Technology Stack

- **Markup**: Semantic HTML5 with ARIA accessibility labels (`role="button"`, `aria-live`, `aria-expanded`).
- **Styling**: Pure Vanilla CSS3 (3D CSS Transforms, `preserve-3d`, `perspective`, CSS Custom Properties, HSL color tokens, `@keyframes`).
- **Scripting**: Pure Vanilla JavaScript (ES6+ modular IIFE architecture).
- **Audio**: Web Audio API (real-time procedural oscillator & noise synthesis).
- **Graphics**: HTML5 `<canvas>` 2D context with device pixel ratio scaling (`window.devicePixelRatio`).
- **Typography**: Google Fonts (*Playfair Display*, *Dancing Script*, *Lato*).
- **Dependencies**: **Zero external libraries or frameworks** — 100% native web technology.

---

## 📁 Project Structure

```
my-project/
├── index.html       # Semantic layout, 3D book structure & controls
├── style.css        # 3D book geometry, leaf physics, lighting & themes
├── app.js           # State machine, audio engine, particles & event system
└── README.md        # Documentation & credits
```

---

## 🚀 Getting Started

### Local Setup
1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/reasons-i-love-you.git
   cd reasons-i-love-you
   ```
2. Open `index.html` directly in any modern web browser (Google Chrome, Mozilla Firefox, Safari, Microsoft Edge):
   - Double-click `index.html`, or
   - Run a local static server:
     ```bash
     npx serve .
     ```

---

## 🎨 Themes Included

Every reason is styled with its own distinct romantic aesthetic:
- 🌹 **Rose Red**: Deep crimson leather & glowing gold borders.
- 🌸 **Blush Pink**: Soft rose quartz & magenta shimmer.
- 🌙 **Midnight Navy**: Sapphire night sky & silver foil.
- 🍑 **Peach Glow**: Warm amber sunrise & sunset gradient.
- 💜 **Lavender Dream**: Royal amethyst & lilac starlight.

---

## 👨‍💻 Author & Credits

- **Creator & Developer**: **hxni**
- **Instagram**: [@the.cipher.stack](https://instagram.com/the.cipher.stack)

> *"In all the world, there is no heart for me like yours."*

---

<p align="center">Made with ❤️ by <b>hxni</b> | Follow on Instagram: <a href="https://instagram.com/the.cipher.stack"><b>@the.cipher.stack</b></a></p>
