# ESP32 Bottango Control Board

This custom PCB is designed to serve as a **control and interface board** for projects using the [Bottango](https://www.bottango.com/) motion and animation control firmware.  
It provides robust connectivity, servo control, and expandability for animatronics or motion-based systems.

---

## Features

### Core
- **ESP32 microcontroller**
- **USB-C** connector for power and programming  
- **Selectable power source** for the ESP32:  
  - USB-C  
  - 5 V rail (from WS2812B)

---

### Inputs
- **4 user buttons** — freely assignable, e.g., for selecting animations  
- **1 stop button** — emergency or animation stop  
- **Potentiometer input** — for audio volume control  

---

### Outputs & Indicators
- **4 status LEDs** — indicate board or animation states  
- **Line-out audio output**  
- **6 servo connectors** (powered by dedicated power input)  
- **WS2812B output** — supports addressable RGB LEDs  
- **Selectable power source for audio section:**  
  - USB-C  
  - 5 V rail (from WS2812B)  
- **LED power indicators** for:  
  - 5 V  
  - 6 V  
  - USB-C  
  - 3.3 V  

---

### Connectivity
- **I²C (Qwiic-compatible connector)** — for sensor or peripheral expansion  
- **RS485 interface** — for robust long-distance serial communication  

---

## Power Overview

| Function             | Voltage  | Source Options               |
|----------------------|----------|------------------------------|
| ESP32                | 5 V      | USB-C / 5 V line             |
| Audio Output Circuit | 5 V      | USB-C / 5 V line             |
| WS2812B LEDs         | 5 V      | External supply              |
| Servos               | 6 V      | External supply              |

---

## Firmware Compatibility

This board is designed for use with **Bottango firmware**, providing smooth integration with Bottango Studio for real-time motion and animation control.  
Learn more at: [https://www.bottango.com/](https://www.bottango.com/)

---

## License

This hardware design is released under the  
**CERN Open Hardware Licence Version 2 – Weakly Reciprocal (CERN-OHL-W)**.  
© 2025 Martin Klein 

You are free to:
- Use, study, modify, and manufacture this design  
- Distribute modified versions under the same license  
- Incorporate this board into larger, closed-source systems, **as long as modifications to this board itself remain open-source**

For more information, see the [LICENSE](./LICENSE) file or the full text at
[https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2](https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2)

## Acknowledgments

Special thanks to the Bottango team for providing an intuitive open platform for animatronic motion control.