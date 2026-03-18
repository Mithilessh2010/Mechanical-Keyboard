
# Mechanical Keyboard

A custom mechanical keyboard with an OLED screen and RGB backlighting.  
Supports MX switches.  
100% keyboard with 103 keys.  

<img width="718" height="474" alt="image" src="https://github.com/user-attachments/assets/31ff8196-36ca-4195-bc41-d4462fea0900" />

## Features

- **OLED screen** for typing speed and lighting control  
- **Open-source firmware** that can be modified

## PCB

- **Custom PCB** with microcontroller  
- **USB-C** connection for power and data

## Case

- **3 parts**: top panel, front piece, back piece  
- Print parts separately and join them  
- Weld front and back pieces  
- Do **not** weld the top panel  
- Minimum printer bed size: **216 x 139 mm**

## Firmware

**Requirements:**  
- CMake  
- GCC  
- arm-none-eabi-gcc  

**Build commands:**
```bash
cmake -S Firmware -B Firmware/build -G "Ninja"
cmake --build Firmware/build --target Keyboard_Firmware
```

**Flashing instructions:**  
- Hold the **BOOT** button and plug the board into your computer  
- The board will appear as a USB drive  
- Drag the `Keyboard_Firmware.uf2` file into the drive  
- The keyboard will reboot and load the firmware  

## Parts List (BOM)

| **Item** | **Link** | **Cost (USD)** | **Qty** | **Total** |
|----------|---------|----------------|---------|-----------|
| **YD-RP2040** | [Link](https://www.aliexpress.com/item/1005006152339711.html) | $3.25 | 1 | $3.25 |
| **74AHCT125** | [Link](https://www.aliexpress.com/item/1005010022053816.html) | $3.30 | 1 | $3.30 |
| **100nF Capacitors** | [Link](https://www.aliexpress.com/item/1005007470747384.html) | $2.00 | 105 | $2.00 |
| **10kΩ Resistors** | [Link](https://www.aliexpress.com/item/1005009805187579.html) | $0.04 | 2 | $0.04 |
| **1N4148 Diodes** | [Link](https://www.aliexpress.com/item/4000685043735.html) | $2.00 | 103 | $2.00 |
| **Hot swap sockets** | [Link](https://www.aliexpress.com/item/1005009594313632.html) | $9.00 | 1 | $9.00 |
| **Gateron Switches** | [Link](https://kurokeeb.com/products/gateron-switch-g-pro-3-0) | $41.20 | 103 | $41.20 |
| **OLED Display 1.5"** | [Link](https://www.aliexpress.com/item/1005009409829497.html) | $4.60 | 1 | $4.60 |
| **SK6812 LEDs** | [Link](https://www.aliexpress.com/item/1005007696173500.html) | $7.40 | 2 | $7.40 |
| **Keycaps** | [Link](https://www.aliexpress.com/item/1005007996240625.html) | $18.50 | 1 | $18.50 |
| **Screws M3x8** | [Link](https://www.aliexpress.com/item/1005008585550992.html) | $0.40 | 8 | $0.40 |
| **Hot melt inserts** | [Link](https://www.aliexpress.com/item/1005006071488810.html) | $1.00 | 8 | $1.00 |
| **Silicone feet** | [Link](https://www.aliexpress.com/item/1005006954839245.html) | $0.80 | 1 | $0.80 |
| **PCB** | [Link](https://www.jlcpcb.com/) | $44.00 | 1 | $44.00 |

**Estimated total: $137**
