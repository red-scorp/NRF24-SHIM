# NRF24-SHIM project

My NRF24-SHIM (mini-HAT) for Raspberry Pi project.

This project came to reality when I was looking for a way to connect standard NRF24L01+ module to my Pi.
I had found many tutorials explaining how to connect NRF24 modules to Pi but no ready made board or even proper schematics.
"Hmm... DIY!" I told myself and here we are.

## NRF24-SHIM

Raspberry Pi 40-pin **NRF24-SHIM** mini-HAT.

Pins Configuration:

|NRF24 Pin|Option 1|Option 2|
|---------|--------|--------|
|CE       |GPIO22\*|GPIO25  |
|CSN      |GPIO8\* |GPIO18  |
|SCK      |GPIO11\*|GPIO21  |
|MOSI     |GPIO10\*|GPIO20  |
|MISO     |GPIO9\* |GPIO19  |
|IRQ      |GPIO23  |GPIO24  |

\*) the pin is connected by default.

## NRF24-mini-SHIM

Raspberry Pi **NTF32-mini-SHIM** micro-HAT.

Pins Configuration:

|NRF24 Pin|Option 1|Option 2|
|---------|--------|--------|
|CE       |GPIO22\*|GPIO25  |
|CSN      |GPIO8\* |        |
|SCK      |GPIO11\*|        |
|MOSI     |GPIO10\*|        |
|MISO     |GPIO9\* |        |
|IRQ      |GPIO23  |GPIO24  |

\*) the pin is connected by default.

## BOM

Bill Of Materials is currently available only for LCSC Electronic Components Distributor, which is probably cheapest anyway.

### LCSC BOM

|Designator     |Part/Value |Package/Footprint |LCSC # |
|---------------|-----------|------------------|-------|
|C1             |Cap. 100nF |0402              |C1525  |
|C2             |Cap. 1uF   |0603              |C15849 |
|R1, R2, R3, R4 |Res. 10K   |0402              |C25744 |

## How to help

Your contributions as code, resources or finances are welcome!
Please contact me directly over e-mail andriy.golovnya@gmail.com or over [GitHub profile](https://github.com/red-scorp).
Link for [Paypal donations](http://paypal.me/redscorp), which are always welcome.
Thanks in advance!
