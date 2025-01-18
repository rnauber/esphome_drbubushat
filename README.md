# esphome_drbubushat
A colorful game for a PhD hat using the M5stack Atom Echo, 8Angle potentiometers, and an addressable LED strip powered through [ESPHome](https://esphome.io/). It is easy to build and requires only minimal soldering! The purpose of the game is to match random colors with their respective positions on a rainbow.

https://github.com/user-attachments/assets/33a868b7-44bc-4bc2-a3f3-f4536aa07cf7

---

## Components

- [M5stack Atom Echo](https://docs.m5stack.com/en/atom/atomecho)  
- [M5stack 8Angle](https://docs.m5stack.com/en/unit/8Angle)  
- [Seeed Grove - WS2813 RGB LED Stripe, waterproof - 30 LED/m](http://www.normandled.com/upload/201605/WS2813%20LED%20Datasheet.pdf)  

---
## Building It

1. Connect the 8Angle potentiometer to the Atom Echo using the Grove connector.
2. Solder the LED strip's wires to a pin header that can be attached to the Atom's GPIOs as follows:

   | LED Strip Pin | Atom Pin |
   |---------------|----------|
   | Gnd           | G        |
   | Vcc           | 5V       |
   | Data          | G25      |

3. Build and flash the ESPHome firmware using the following command:  
   ```bash
   esphome run drbubushat.yaml

  ```
   
