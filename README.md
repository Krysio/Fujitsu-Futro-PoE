# Fujitsu Futro PoE Module Pinout

This repository documents the pinout of the 20-pin PoE connector found in Fujitsu Futro devices.

## 20-pin Connector Pin Layout

Below is the pin layout for the PoE connector, which includes both power, PCIe, and unknown pins. This can be useful for modding or repurposing the connector for custom PCIe 1x expansion.

|   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|
| PowrGD# | Vcc 3.3V | Wake# | PoE 19V | PoE 19V | PoE 19V | Unknown | Unknown | Unknown | Unknown |
| GND     | TX-      | TX+   | GND     | RX-     | RX+     | GND     | CLK-    | CLK+    | GND     |

![Pins of PoE connector](./FutroPOE.jpg?raw=true "Pins of PoE connector")
![A test adapter made with a motherboard USB3 connector](./FutroUSB3Connector.jpg?raw=true "A test adapter made with a motherboard USB3 connector")

## License
This project is licensed under the MIT License. Feel free to use and modify the content.
