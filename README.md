# LED Matrix Editor & Animator 🎨✨

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![FastLED Compatible](https://img.shields.io/badge/FastLED-Compatible-brightgreen.svg)](https://github.com/FastLED/FastLED)
[![ESP32 Bluetooth](https://img.shields.io/badge/ESP32-Web%20Bluetooth-blue.svg)](https://espressif.com/)
[![Support on Ko-fi](https://img.shields.io/badge/Support-Ko--fi-ff5e5b.svg)](https://ko-fi.com/deadline73083)

A lightweight, standalone, zero-dependency web application for designing, animating, and deploying LED matrix animations to WS2812B / NeoPixel strips and matrices via **FastLED** and direct **Web Bluetooth (BLE)**.

Designed for makers, electronics hobbyists, and DIY LED enthusiasts.

---

## 🌟 Key Features

- **Standalone & Offline-Ready**: Completely contained in a single `index.html` file. No build steps, no Node.js required. Open directly in any modern browser or host via GitHub Pages.
- **Canvas & Matrix Geometry**:
  - Configurable width and height (from 1x1 up to 64x64).
  - Quick presets: `8x8`, `16x16`, `32x32`, `8x32`.
  - Wiring layout options: **Linear**, **Serpentine**, or **Custom Map** (interactive visual pixel-by-pixel mapper).
  - Hardware rotation: `0°`, `90°`, `180°`, `270°`.
  - Color order configurations: `RGB`, `GRB`, `BRG`, `RBG`, `GBR`, `BGR`.
- **Drawing Tools & Palette**:
  - Pencil, flood fill, eraser, eyedropper (pipette).
  - Custom color picker (RGB sliders + Hex input).
  - Editable color palette swatches.
- **Animation Timeline**:
  - Multi-frame animation editor with per-frame custom FPS.
  - Frame duplicate, copy/paste, clear, and drag-and-drop reordering.
  - Frame transformations: shift (Up/Down/Left/Right) and flip (Horizontal/Vertical).
  - **Onion Skinning**: Auto (previous frame) or pinned reference frame.
  - Real-time animated preview with play/pause.
- **Export & Firmware Integration**:
  - **Arduino / FastLED Code Generator**: Generates production-ready C++ code with optional `PROGMEM` and diff/delta compression.
  - **Ready-to-Use ESP32 BLE Firmware**: Built-in firmware template with automatic PSRAM and internal SRAM heap fallback.
  - **Direct Upload via Web Bluetooth**: Upload animations wirelessly from your browser (Chrome/Edge on Android, Windows, Mac, Linux) directly to an ESP32 receiver.
- **Project Save & Load**:
  - Export project as `.json` file and reload anytime.
  - Auto-saved preferences in browser `localStorage`.

---

## 🚀 Quick Start

### 1. Run Online or Locally
- **Direct in Browser**: Double-click `index.html` to open it locally in Google Chrome or Microsoft Edge.
- **GitHub Pages**: Fork or push this repository and enable GitHub Pages in Settings -> Pages -> Deploy from branch (`main` / `master`).

### 2. Wireless Upload to ESP32 via Bluetooth
1. Click **"💾 Copy ESP32 Firmware"** in the Code & Upload section.
2. Open Arduino IDE, install the `FastLED` library, paste the code into an ESP32 sketch, and flash your ESP32 board.
3. Power on the ESP32 and ensure Bluetooth is enabled on your computer or phone.
4. Draw your animation in the editor, set the desired FPS, and click **"⚡ Send via BT"**.
5. Select your ESP32 device from the browser popup. The animation will be uploaded wirelessly and play immediately!

---

## ☕ Support the Project

If you find this tool helpful for your DIY and maker projects, you can support further development:

[![Support on Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/deadline73083)

**Ko-fi**: [https://ko-fi.com/deadline73083](https://ko-fi.com/deadline73083)

---

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**.

- **You are free to**:
  - **Share** — copy and redistribute the material in any medium or format.
  - **Adapt** — remix, transform, and build upon the material.
- **Under the following terms**:
  - **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.
  - **NonCommercial** — You may **not** use the material for commercial purposes or monetization.

See the [LICENSE](LICENSE) file for complete details.
