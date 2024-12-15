# EasyThreed-K7-Display-Upgrade

<img src="https://i.ibb.co/YcPMHd1/Easy-Threed-K7-with-LCD-WM.jpg" alt="MicroSD Card 4GB" width="150"/>

## This is a guide to adding an LCD display to the EasyThreed K7 printer.

> [!IMPORTANT]
> This is an **unofficial firmware update** and **not supported by EasyThreed**. It was created as a community project to enhance the functionality of the EasyThreed K7 printer. Use it at your own risk. Any issues that arise from the use of this firmware are not the responsibility of the original manufacturer.

### Description

This project provides an upgrade solution for the **EasyThreed K7 3D printer** by adding **LCD display *(RepRapDiscount Full Graphic Smart Controller)***, powered by a customized Marlin firmware. The firmware enables full display support in **English** or **Czech** language and enhances usability for EasyThreed K7 owners.

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

### Limitations and Known Issues:

- **SD card support:** The display does not support SD card slot functionality. Therefore, you will need to continue using the original SD card slot on the printer for file management and printing.
- **Display case weakness:** The display case has relatively thin walls. It's recommended to reinforce them with glue to improve durability and prevent potential damage during use.

> [!NOTE]
> Apologies for not including detailed photos of the display attachment process; I hope the provided instructions and diagrams are clear enough to guide you through the installation.

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
	- Start by unscrewing the **four screws** that secure the bottom cover of the printer.
	- Once the cover is removed, locate the **14-pin connector** labeled **EXP1**. This is where the LCD display will be connected to the mainboard.
	- <br><img src="https://i.ibb.co/dpxbZjm/exp1-easythreed-k7.jpg" alt="EXP1 connector" width="250"/>
	<br>*Image Credit: mysku.ru*
	
3. **Connect the LCD Display Using DuPont Wires:**
	- Carefully remove the existing connector from the **EXP1** port on the mainboard.
	- Use the DuPont cables to connect the LCD display to the **EXP1** port according to the wiring diagram.
	- <br><img src="https://i.ibb.co/KVqzP4t/Easy-Threed-K7-schematic.jpg" alt="EXP1 connector" width="500"/><br>
> [!WARNING]
> Ensure that the DuPont connectors are securely attached and double-check the wiring to avoid incorrect connections, as improper wiring could permanently damage one of the components.

4. **Test the Display:**
	- **Power on** the printer. You should first see the **EasyThreed logo**, followed by the **Marlin logo**, and then the **main screen**.
	- **Test** the functionality by navigating through the **menu** (e.g. **axis movement**, **home position**, etc.).
	- If there are issues with the display, **recheck the wiring connections** and ensure the **firmware update** was applied correctly.
> [!TIP]
> It's a good idea to print a small test object to verify that everything is functioning correctly. This will help ensure that your upgraded display is properly communicating with the printer and that the printer is operating as expected after the firmware update.

5. **Reassemble the Printer:**

	- After confirming that the **display** is working correctly, it's time to **reassemble** your EasyThreed K7. If you have **long enough DuPont cables** that can reach the front of the printer, you can use this option to make the connections. However, I personally used the **cables provided** with the display, which I **cut in the middle** and **soldered DuPont cables** to extend them. If you decide to use this method, you’ll need to **check the pinout** using a **multimeter** to identify which lead corresponds to which function.
	- **Peel off the EasyThreed logo** from the front of the printer.
	- **Drill two holes** in the printer according to the size of the printed **holder** for the display.
	- **Secure the display** in place using **screws**. If necessary, you can use **superglue** to ensure the display stays in place if it doesn’t hold firmly enough.
	- After everything is mounted, **reconnect any cables** that were unplugged during the installation process.
	- **Reinstall the bottom cover** and secure it with screws.


------------

> [!NOTE]
> I want to emphasize once again that some of the solutions I have chosen may not be the ideal choice for everyone, but I selected them based on my own preferences and experiences. If they don't suit you, feel free to adjust them according to your needs.

### Recovery and Original Firmware:

- If something goes wrong or you wish to revert to the original firmware, you can download the official firmware for the EasyThreed K7 printer from [this link](insert link here). Be sure to follow the manufacturer's instructions for installation to avoid any issues.
