⌨️ Keyboard Project: Prototype Carbon
A custom 65% keyboard with 3u split spacebars

🛠️ How to Build This Keyboard
1. 🧾 Print the PCB
📂 View PCB Gerber Files

2. 🖨️ Print the Case and Plates
📐 View Acrylic Shell Stack (DWG)

🔩 View Positioning Plate (DWG)

3. 🔌 Order Electrical Components
📄 View Bill of Materials (BOM)
Plus additionally:

1x ATmega32u4AU microcontroller

67x Kailh hot swap sockets

67x 6028RGBC-WS2812B RGB LEDs

4. 🎹 Buy Keyboard Parts
67x hot-swappable mechanical switches (any type)

67x keycaps of your choice

24x M2 x 4mm screws

12x M2 x 14mm double-headed copper standoffs

5. 🔧 Assembly Instructions
Refer to the PCB while soldering — make sure all components are in the correct orientation

Double-check LED and MCU pin alignment

6. 💻 Compile the Firmware
Use QMK_MSYS

📁 View firmware folder

7. 🚀 Flash the Firmware
Upload your compiled .hex or .bin file using QMK Toolbox

🐞 Known Issues
❗ EC11 Rotary Encoder Not Properly Implemented
One of the encoder pins connects to the AREF pin on the ATmega32u4AU.

⚠️ Do not install the EC11 rotary encoder unless you’ve fixed this in hardware.
Use a standard hot swap socket in its place for now.
