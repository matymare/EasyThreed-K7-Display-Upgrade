# EasyThreed-K7-Display-Upgrade

<img src="https://i.ibb.co/YcPMHd1/Easy-Threed-K7-with-LCD-WM.jpg" alt="MicroSD Card 4GB" width="150"/>

## This is a guide to adding an LCD display to the EasyThreed K7 printer.

### Description

This project provides an upgrade solution for the **EasyThreed K7 3D printer** by adding a functional **LCD display *(RepRapDiscount Full Graphic Smart Controller)***, powered by a customized Marlin firmware. The firmware enables full display support in **English** or **Czech** language and enhances usability for EasyThreed K7 owners.

> [!NOTE]
> This solution may not be the ideal choice for everyone, but it works well for my setup, and I considered it the most suitable solution for my needs. Feel free to modify and adapt it according to your own preferences and requirements.

### Key Features
- **Custom Marlin Firmware:** Adds full support for an LCD display, enhancing printer usability.
- **Multilingual Support:**
	- **English** (primary language)
	- **Czech** (additional localized option)
- **Precompiled Binary:** Ready-to-install firmware (mksLite.bin) for quick flashing.
- **User-Friendly Installation:** Simple step-by-step guide provided for easy setup.
- **3D Model Files:**
	- Custom parts I designed specifically for this project.
	- Other compatible components sourced and reused to complete the enclosure.
	- All models can be printed directly on the EasyThreed K7 printer.

### Requirements

| Item name | Where to buy | Image |
| ------------ | ------------ | ------------ |
| **EasyThreed K7 3D Printer** | [Search for EasyThreed K7 on Google](https://www.google.com/search?q=buy+EasyThreed+K7) | <img src="https://i.ibb.co/5xrZpV7/Easy-Threed-K7.jpg" alt="EasyThreed K7" width="75"/> |
| **RepRapDiscount Full Graphic Smart Controller** | [Search for this RepRap LCD on Google](https://www.google.com/search?q=buy+RepRapDiscount+Full+Graphic+Smart+Controller) | <img src="https://i.ibb.co/7jLRqm6/Rep-Rap-Discount-Full-Graphic-Smart-Controller.jpg" alt="EasyThreed K7 Display" width="75"/> |
| **12x F-F DuPont Wires** | [Search for F-F DuPont Wires on Google](https://www.google.com/search?q=buy+F-F+DuPont+Wires) | <img src="https://i.ibb.co/6RcWCrQ/F-F-Du-Pont-Wires.jpg" alt="F-F DuPont Wires" width="75"/> |
| **Micro SD Card (I used 4GB)** *- for upload the update file to the printer* | [Search for MicroSD Card 4GB on Google](https://www.google.com/search?q=buy+MicroSD+Card+4GB) | <img src="https://i.ibb.co/k9tsPNY/micro-SD-card-4-GB.jpg" alt="MicroSD Card 4GB" width="75"/> |
| **8x 16mm M3 bolts and nuts** | [Search for 16mm M3 bolts and nuts on Google](https://www.google.com/search?q=buy+16mm+M3+bolts+and+nuts) | <img src="https://i.ibb.co/jLrYy0C/M3-16mm-bolt-and-nut.jpg" alt="16mm Bolt and Nuts" width="75"/> |

### Additional Requirements

- **Screwdrivers** for assembly and dismantling
- **Solder and soldering iron** for soldering wires to cable
- **Drill** for making holes in the printer to mount the display.
- **Handy hands 🙂**

------------

## Installation Guide
Follow these steps to upgrade your EasyThreed K7 with the new display:

> [!TIP]
> Before starting the upgrade, print all necessary 3D parts (such as the display box and holder) while your printer is still fully assembled. Upgrading the printer may involve partial disassembly, which could make it difficult or impossible to print parts afterward. You can find the required 3D models on [Thingiverse](https://www.thingiverse.com/thing:6873216) Preparing these components beforehand will save time and help you avoid unnecessary complications during the upgrade process.

1. **Download the Firmware:**
	- Choose the appropriate firmware file (`mksLite.bin`) from this repository based on your preferred language (e.g., English or Czech).
	- Format a microSD card as FAT32 and copy the `mksLite.bin` file onto it. Ensure no other files are on the card to prevent potential conflicts during the update.
	- Insert the microSD card into the printer **while it is powered off**, then turn on the printer. Wait for less than 30 seconds while the firmware installs automatically.
	- After the update is complete, the firmware file on the SD card will be renamed to `mksLite.cur`, indicating a successful installation.

2. **Remove the Bottom Cover and Access the EXP1 Connector:**
	- Start by unscrewing the four screws that secure the bottom cover of the printer.
	- Once the cover is removed, locate the **14-pin connector** labeled **EXP1**. This is where the LCD display will be connected to the mainboard.
	- <br><img src="https://i.ibb.co/dpxbZjm/exp1-easythreed-k7.jpg" alt="EXP1 connector" width="250"/>
	<br>*Image Credit: mysku.ru*
	
3. **Connect the LCD Display Using DuPont Wires**
	- Carefully remove the existing connector from the EXP1 port on the mainboard.
