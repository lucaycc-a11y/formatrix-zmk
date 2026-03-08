# ForMatrix (Caldera) ZMK Config

ZMK firmware configuration for **ForMatrix** keyboard, based on the Caldera split keyboard design.

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

## Build via GitHub Actions

1. Push this repo to GitHub
2. Go to Actions tab
3. Run the build workflow
4. Download the firmware files

## Flashing

### First Time (requires reset button or double-tap)

1. Connect left half via USB
2. Double-tap reset button OR short RST to GND
3. A USB drive will appear
4. Copy `caldera_left_studio.uf2` to the drive
5. Repeat for right half with `caldera_right.uf2`

### After First Flash

Use **Layer 3** (hold LOWER + RAISE) to enter bootloader mode!

## ZMK Studio

1. Flash the left half with the "studio" firmware
2. Connect via USB
3. Open [ZMK Studio](https://zmk.studio/)
4. Edit your keymap live!

## Bluetooth Pairing

- Layer 2 has BT1-BT5 keys
- Press BT_CLR to clear all bonds
- Press BT_SEL 0-4 to switch profiles

## Keymap

```
Layer 0 (Default):
┌─────┬─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┬─────┐
│ ESC │  1  │  2  │  3  │  4  │  5  │   │  6  │  7  │  8  │  9  │  0  │BKSP │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB │  Q  │  W  │  E  │  R  │  T  │   │  Y  │  U  │  I  │  O  │  P  │  \  │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│CAPS │  A  │  S  │  D  │  F  │  G  │   │  H  │  J  │  K  │  L  │  ;  │  '  │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHFT │  Z  │  X  │  C  │  V  │  B  │   │  N  │  M  │  ,  │  .  │  /  │ ENT │
├─────┼─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │ GUI │ ALT │  `  │LOW ↓│ SPC │   │ SPC │RAIS ↑│  -  │  =  │  [  │  ]  │
└─────┴─────┴─────┴─────┴─────┴─────┘   └─────┴─────┴─────┴─────┴─────┴─────┘
```

## Credits

- Based on [Caldera Keyboard](https://github.com/christianselig/caldera-keyboard) by Christian Selig
- Built with [ZMK Firmware](https://zmkfirmware.dev/)

---

**FORM LABS** — LOGIC TAKES FORM
