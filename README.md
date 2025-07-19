# ⌨️ Keyboard Project: Prototype Carbon

A custom **65% keyboard** with **3u split spacebars**.
# Watch Demo!
[![Watch Video](https://img.youtube.com/vi/WMbd48JGXQo/hqdefault.jpg)](https://www.youtube.com/watch?v=WMbd48JGXQo&ab_channel=XinlinWu)
---

## 🛠️ How to Build This Keyboard

### 1. 🧾 Print the PCB
- [📂 View PCB Gerber Files](./Gerber_prototypeCarbon_PCB_prototypeCarbon_2025-07-03.zip)

### 2. 🖨️ Print the Case and Plates
- [📐 Acrylic Shell Stack (DWG)](./prototypeCarbonGasketShell.dwg)  
- [🔩 Positioning Plate (DWG)](./gasket.dwg)

### 3. 🔌 Order Electrical Components
- [📄 BOM Sheet](./BOM_prototypeCarbon_2025-07-03.csv)

Additional components not in the BOM:
- `1x` ATmega32u4AU microcontroller  
- `67x` Kailh hot swap sockets  
- `67x` 6028RGBC-WS2812B RGB LEDs

### 4. 🎹 Buy Keyboard Parts
- `67x` hot-swappable mechanical switches (any type)  
- `67x` keycaps of your choice  
- `24x` M2 x 4mm screws  
- `12x` M2 x 14mm double-headed copper standoffs

### 5. 🔧 Assemble the Keyboard
- Refer to the PCB while soldering — **ensure all components are correctly oriented**
- Pay special attention to LED and MCU pin alignment

### 6. 💻 Compile the Firmware
- Use **QMK_MSYS** to compile the firmware  
- [📁 View Firmware Directory](./qmk_firmware/keyboards/prototypeCarbon)

### 7. 🚀 Flash the Firmware
- Use **QMK Toolbox** to upload the compiled firmware to the keyboard

### 8. 🧩 Upload Keyboard Layout to VIA to view Keymap and Keybinds
- [📁 View Layout Json](./prototypeCarbonVIA.json)
---

## 🐞 Known Issues

- ❗ **EC11 Rotary Encoder Pin Error**  
  The EC11 rotary encoder is **not implemented correctly** on the PCB — one of its pins is connected to the **AREF** pin on the ATmega32u4AU.

  > ⚠️ **Do not install** the EC11 rotary encoder unless you have fixed this in hardware.  
  Instead, use a regular hot swap socket in its place.
