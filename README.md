# Fujitsu Futro PoE Module Pinout

This repository documents the pinout of the 20-pin PoE connector found in Fujitsu Futro devices.

## 20-pin Connector Pin Layout

The PoE connector has a 2 mm pitch. I used a blue 20-pin USB 3.0 connector for my adapter.

Below is the pin layout for the PoE connector, which includes both power, PCIe, and unknown pins. This can be useful for modding or repurposing the connector for custom PCIe 1x expansion.

|   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|
| PowrGD# | Vcc 3.3V | Wake# | PoE 19V | PoE 19V | PoE 19V | Unknown | Unknown | Unknown | Unknown |
| GND     | TX-      | TX+   | GND     | RX-     | RX+     | GND     | CLK-    | CLK+    | GND     |

![Pins of PoE connector](./FutroPOE.jpg?raw=true "Pins of PoE connector")

The `PowrGD#` signal should be used as the `PERST#` signal.
When the device is running, a 19V voltage appears on the pins labeled `PoE 19V`.

## Power supply via PoE

I haven't worked on it.

## Examples

![A test adapter made with a motherboard USB3 connector](./FutroUSB3Connector.jpg?raw=true "A test adapter made with a motherboard USB3 connector")
![An adapter to PCIe 1x connector](./Adapter2PCIe1x.jpg?raw=true "An adapter to PCIe 1x connector")

An adapter to M2 key M for a NVMe drive:

[Router/firewall/NAS DIY na terminalu Fujitsu FUTRO S940. Czy się uda?](https://eko.one.pl/forum/viewtopic.php?pid=312550#p312550)

Fujitsu FUTRO S940 supports NVMe in the PoE connector.

## See also
[Fujitsu Futro s920, the second ethernet connector](https://github.com/Krysio/Fujitsu-Futro-s920-second-ethernet)

## License
This project is licensed under the MIT License. Feel free to use and modify the content.
