# NRF24-SHIM project

NRF24-SHIM (mini-HAT), an interface board for NRF32L01+ radio boards for Raspberry Pi.

This project came to reality when I was looking for a way to connect standard NRF24L01+ module to my Pi.
I had found many tutorials explaining how to connect NRF24 modules to Pi but no ready made board or even proper schematics.
"Hmm... DIY!" I've told myself and here we are.

## NRF24-SHIM

Raspberry Pi 40-pin **NRF24-SHIM** mini-HAT.

Preview:

![NRF24-SHIM preview](img/NRF24-SHIM.png)

[Schematics in PDF format](doc/NRF24-SHIM.pdf)

Features:

- locked Pi headers
- locked NRF24 headers
- double set of Pi headers (for inside and outside mount)
- SPI0/SPI1 bus selection
- CE/IRQ selection
- can be used as SHIM (no headers) or HAT (with headers)

Pins Configuration:

|NRF24 Pin |Option 1 |Option 2 |
|----------|---------|---------|
|CE        |GPIO22\* |GPIO25   |
|CSN       |GPIO8\*  |GPIO18   |
|SCK       |GPIO11\* |GPIO21   |
|MOSI      |GPIO10\* |GPIO20   |
|MISO      |GPIO9\*  |GPIO19   |
|IRQ       |GPIO23   |GPIO24   |

\*) the pin is connected by default.

CAM files are available.

## NRF24-mini-SHIM

Raspberry Pi **NTF32-mini-SHIM** micro-HAT.

Preview:

![NRF24-mini-SHIM preview](img/NRF24-mini-SHIM.png)

[Schematics in PDF format](doc/NRF24-mini-SHIM.pdf)

Features:

- locked Pi headers
- locked NRF24 headers
- CE/IRQ selection
- very small size
- fits on 26- and 40-pin Pi headers

Pins Configuration:

|NRF24 Pin |Option 1 |Option 2 |
|----------|---------|---------|
|CE        |GPIO22\* |GPIO25   |
|CSN       |GPIO8\*  |         |
|SCK       |GPIO11\* |         |
|MOSI      |GPIO10\* |         |
|MISO      |GPIO9\*  |         |
|IRQ       |GPIO23   |GPIO24   |

\*) the pin is connected by default.

CAM files are available.

## NRF24-zero-SHIM

Raspberry Pi zero 40-pin **NRF24-zero-SHIM** mini-HAT.

Preview:

![NRF24-zero-SHIM preview](img/NRF24-zero-SHIM.png)

[Schematics in PDF format](doc/NRF24-zero-SHIM.pdf)

Features:

- locked Pi headers
- locked NRF24 headers
- Pi zero board style
- SPI0/SPI1 bus selection
- CE/IRQ selection
- double NRF24 configuration possible
- can be used as SHIM (no headers) or HAT (with headers)

Pins Configuration:

|NRF24 Pin |Option 1 |Option 2 |Option 3 |Option 4 |Option 5 |
|----------|---------|---------|---------|---------|---------|
|P0 CE     |GPIO22\* |GPIO25   |GPIO27   |         |         |
|P0 CSN    |GPIO8\*  |GPIO7    |GPIO18   |GPIO17   |GPIO16   |
|P0 SCK    |GPIO11\* |GPIO21   |         |         |         |
|P0 MOSI   |GPIO10\* |GPIO20   |         |         |         |
|P0 MISO   |GPIO9\*  |GPIO19   |         |         |         |
|P0 IRQ    |GPIO23   |GPIO24   |         |         |         |
|P1 CE     |GPIO22   |GPIO25\* |GPIO27   |         |         |
|P1 CSN    |GPIO8    |GPIO7    |GPIO18\* |GPIO17   |GPIO16   |
|P1 SCK    |GPIO11   |GPIO21\* |         |         |         |
|P1 MOSI   |GPIO10   |GPIO20\* |         |         |         |
|P1 MISO   |GPIO9    |GPIO19\* |         |         |         |
|P1 IRQ    |GPIO23   |GPIO24   |         |         |         |

\*) the pin is connected by default.

CAM files are available.

## BOM

Bill Of Materials is currently available only for LCSC Electronic Components Distributor, which is probably cheapest anyway.

### LCSC BOM

|Designator                      |Part/Value |Package/Footprint |LCSC # |
|--------------------------------|-----------|------------------|-------|
|C1, C3\*                        |Cap. 100nF |0402              |C1525  |
|C2, C4\*                        |Cap. 1uF   |0603              |C15849 |
|R1, R2, R3, R4, R5, R6, R7, R8\*|Res. 10K   |0402              |C25744 |

\*) These passive components are optional but it's recommended to install them.

## Links

- [pinout.xyz](https://pinout.xyz/) - a brilliant resource on topic of Pi's pinout and HATs.
- [raspberrypi/hats](https://github.com/raspberrypi/hats) - Pi's HAT specification.
- [Communication between Arduino AND Raspberry Pi using NRF24L01](https://medium.com/@anujdev11/communication-between-arduino-and-raspberry-pi-using-nrf24l01-818687f7f363) - how to setup NRF24L01 with Pi.
- [Funkkommunikation zwischen Raspberry Pi’s und Arduinos (2.4 GHz)](https://tutorials-raspberrypi.de/funkkommunikation-zwischen-raspberry-pis-und-arduinos-2-4-ghz/) - how to setup NRF24L01 with Pi in German.
- [Connecting an nRF24L01+ to Raspberry Pi](https://www.hackster.io/wirekraken/connecting-an-nrf24l01-to-raspberry-pi-9c0a57) - one more setup example.

## How to help

Your contributions as code, resources, or finances are welcome! Please contact me directly via email at andriy.golovnya@gmail.com or through my [GitHub profile](https://github.com/red-scorp).

If you'd like to make a financial contribution, you can donate via [PayPal](http://paypal.me/redscorp) or [Ko-Fi](http://ko-fi.com/redscorp). Your support is greatly appreciated.

Thanks in advance!
