# Kirigami PCB Mod

![Overview of the PCB's](/Images/overview.png?raw=true "Title")

This mod adds two PCBs ([Frame PCB](#frame-pcb), [Kirigami PCB](#kirigami-pcb)) and a cable ([Cable](#cable-and-chain)) to the V0.1/V0.2 that can aid in wire management and routing.

There are also optional things like a [Bed Fan](https://github.com/livinhack/Kirigami_PCB/tree/main/Optional/Bed_Fan) or a [Kirigami-Front](https://github.com/livinhack/Kirigami_PCB/tree/main/Optional/Front).

----

# Frame PCB
The frame PCB mounts on the side in the electronics bay of the printer and combines all cables into a single 10 pin Micro-Fit 3.0 connector. (With neopixel loop-through.)


![Alt text](Images/frame_pcb.png?raw=true "Title")

## Frame PCB BOM
| Part                        | Quantity V1/V2 | Notes           | LCSC Part Number | Link                                                                                                               |
| --------------------------- |      :-:       | --------------- | ---------------- |------------------------------------------------------------------------------------------------------------------- |
| 10 Pin Socket (Right Angle) | 1              | MOLEX 430451000 | C122421          | [lcsc](https://www.lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_MOLEX-430451000_C122421.html)              |
| 2 pin JST XH                | 2              | 2.5mm pitch     | C158012          | [lcsc](https://lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_JST-Sales-America-B2B-XH-A-LF-SN_C158012.html) |
| 3 pin JST XH                | 2              | 2.5mm pitch     | C144394          | [lcsc](https://lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_JST-Sales-America-B3B-XH-A-LF-SN_C144394.html) |
| Screw Terminal              | 1              | 5.08mm pitch    |                  | [digikey](https://www.digikey.de/en/products/detail/metz-connect-usa-inc/31101102/7794830)                                    |
| Screw M3x8                  | 2              |                 |                  |                                                                                                                    |
| Nut M3                      | 2              |                 |                  |                                                                                                                    |
----

# Kirigami PCB

Mounted on the Kirigami bed mount, this breaks out the 10 pin harness into all needed connectors.
For the RGB lovers among us: [U.F.O.](https://github.com/livinhack/Kirigami_U.F.O)

![Alt text](Images/kirigami_pcb.png?raw=true "Title")


## Kirigami PCB BOM
| Part                        | Quantity V1 | Quantity V2 | Notes           | LCSC Part Number | Link                                                                                                               |
| --------------------------- |     :-:     |     :-:     | --------------- | ---------------- |------------------------------------------------------------------------------------------------------------------- |
| 10 Pin Socket (Right Angle) | 1           | 1           | MOLEX 430451000 | C122421          | [lcsc](https://www.lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_MOLEX-430451000_C122421.html)              |
| 2 pin JST XH                | 4           | 3           | B2B-XH          | C158012          | [lcsc](https://lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_JST-Sales-America-B2B-XH-A-LF-SN_C158012.html) |
| 4 pin JST XH                | 1           | 1           | B4B-XH          | C144395          | [lcsc](https://lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_JST-Sales-America-B4B-XH-A-LF-SN_C144395.html) |
| Screw Terminal              |             | 1           | 5.08mm pitch    |                  | [digikey](https://www.digikey.de/en/products/detail/metz-connect-usa-inc/31101102/7794830)                                    |
| Screw M3x6                  | 8           | 8           | *(Or M3x8)*     |                                                                                                                                       |
| Heat-Set Inserts            | 8           | 8           | Voron-spec      |                                                                                                                                       |

### Optional Parts
| Part                | Quantity | Notes                            | LCSC Part Number | Link                                                                                                                             |
| ------------------- |   :-:    | -------------------------------- | ---------------- |--------------------------------------------------------------------------------------------------------------------------------- |
| 0805 10uF Capacitor |  1       | Use if using BARE neopixel IC's. | C162422           | [lcsc](https://www.lcsc.com/product-detail/_Murata-Electronics-_C162422.html) |

## [Optional Bed Fan](https://github.com/livinhack/Kirigami_PCB/tree/main/Optional/Bed_Fan)

## [Optional Front](https://github.com/livinhack/Kirigami_PCB/tree/main/Optional/Front)

### If you have a Neopixel in your Kirigami front, please note the following:
![Alt text](/Images/pixelwire.png?raw=true "Title")
---

# Cable and chain

The Cable is a dual ended 10P (2x5) microfit cable. The connectors are wired 1:5, 6:10 so pin 1 connects to pin 5, pin 2 connects to pin 4 and so forth for all 10 pins.


*Only 2 of the 10 wires are shown for clarity. Connect each number to its opposite. (in it's row!)*

![Alt text](Images/connector.png?raw=true "Title")

Symbolic representation of the connection:

![Alt text](Images/wiring_example.png?raw=true "Title")

## Cable BOM
| Part           | Quantity | Notes                                          | LCSC Part Number | Link                                                                                             |
| -------------- |    :-:   | ---------------------------------------------- | ---------------- |------------------------------------------------------------------------------------------------- |
| 10 Pin Plug    | 2        | Molex 430251400                                | C259745          | [lcsc](https://www.lcsc.com/product-detail/Rectangular-Connectors-Housings_MOLEX-430251000_C259745.html) |
| Microfit Crimp | 20       | Molex 430300001                                | C259786          | [lcsc](https://lcsc.com/product-detail/Line-Pressing-Terminals_MOLEX-430300001_C259786.html)             |
| Wire           | 10       | Smallest required AWG per respective function. |                  | PTFE/Silicone/Hefulon for motion rated                                                           |
### Note: Don't use 20 AWG wire on all ten!(!!!) It works, but it's a s**t job... Ask me how I know...
![Alt text](Images/IGUS_open_chain.png?raw=true "Title")

### Note: You don't need the chain-end spacer if your chain is "V0.1-spec"!
| Part  | Part Number  | Link                                                                                |
| ------| ------------ |------------------------------------------------------------------------------------ |
| Chain | E04.07.015.0 | [fermio](https://www.fermio.shop/igus-gmbh/igus-e-chain-e04.07-15-chain-links-open/)          |
|       |              | [igus](https://www.igus.eu/iPro/iPro_01_0009_0001_GBen.htm?ArtNr=E04.07.015.0&c=DE&l=en)    |
|       |              | [lecktor](https://lecktor.com/en/v0-cables-connectors/716-igus-v02-chain-e04070150-00716.html) |

-----

# Change Log #


## V2+:
 - Link to U.F.O. variant
 - 
## V2:
 - Moved Screw Terminal postition on Frame PCB and rearranged positons of the connectors + changing heater to Screw Terminal on the Kirigami PCB

## V1:
 - Initial Idea
