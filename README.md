# ForMatrix (Caldera-based) ZMK Config

ZMK firmware configuration for **ForMatrix** keyboard.

## Features

- **3 Layers:**
  - Layer 0: Default QWERTY
  - Layer 1: Function keys + Symbols
  - Layer 2: Bluetooth selection + Settings
  - Layer 3: Reset (hold LOWER + RAISE)

- **ZMK Studio Support** - Live keymap editing via USB
- **Bluetooth Auto-Reconnect** - Remembers up to 5 devices
- **Battery Monitoring** - Voltage reporting enabled
- **Deep Sleep** - Saves battery when idle

## Hardware

- **MCU:** nice!nano v2 / Pro Micro nRF52840 / Supermini nRF52840
- **Layout:** Split keyboard (5×6 per side)
- **PCB:** Based on [Caldera Keyboard](https://github.com/christianselig/caldera-keyboard)

## Build

Push to GitHub → Actions will auto-build firmware

## Artifacts

- `formatrix_left_studio.uf2` - Left half with ZMK Studio
- `formatrix_right.uf2` - Right half
- `formatrix_settings_reset.uf2` - Settings reset utility

## Flashing

1. Double-tap reset button OR short RST to GND
2. Copy `.uf2` file to the USB drive that appears
3. Done!

## ZMK Studio

1. Flash left half with `formatrix_left_studio.uf2`
2. Connect via USB
3. Open [ZMK Studio](https://zmk.studio/)
4. Edit your keymap live!

---

**FORM LABS** — LOGIC TAKES FORM
