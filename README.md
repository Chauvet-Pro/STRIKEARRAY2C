# STRIKEARRAY2C

## Software Versions

[V1.0.4 - STRIKE Array 2C](https://github.com/Chauvet-Pro/STRIKEARRAY2C/blob/83eea2cf1771d7f5d01e2be268fad7ce3742897d/Firmware/V1.0.4_07-24-25.zip)
- Expands sACN Universe Limit and optimizes fan control

[V1.0.3 - STRIKE Array 2C](https://github.com/Chauvet-Pro/STRIKEARRAY2C/blob/eb09c532f0f56f60f0e6496f74fd45d26bf62b2a/Firmware/V1.0.3_04-23-25.zip)
- Fixes sACN bug found in v1.0.2

[V1.0.2 - STRIKE Array 2C](https://github.com/Chauvet-Pro/STRIKEARRAY2C/blob/d6f77680d081bebbcd1b15952fcaf151ac95196d/Firmware/V1.0.2_04-11-25.zip)
- Added the 2ch and 8ch mode (duplicate the 2ch and 8ch modes from the Strike Array 2)
- Fixed the Auto Programs 4, 5, 6 out of sync issue.  
- Moved the temperature and battery capacity icons down a bit.
- Changed the Control Channel according to the Well series.
- Added the sub-net mask
- Revised the linear response speed of low-end dimming brightness
- Changed the function and information in the Web-server
- Changed the starting channel settings for Ethernet
- Updated the USB upgrade function, only works when enter the USB upgrade interface 


[V1.0.1 - STRIKE Array 2C](https://github.com/Chauvet-Pro/STRIKEARRAY2C/blob/27c99477dc3e1c45bc11e609be987f870453869d/Firmware/V1.0.1_04-29-24.zip)
- Released software version

&nbsp;

## USB Software Update Instructions
1. Power on the product and plug the flash drive into the USB port.
2. Once the flash drive has been detected, the message "**Upgrade Firmware**" will be displayed. Press **< ENTER >**.
   >* If a different message appears on the display, search for the updated software in the main menu (**Update Firmware**) and select from ***Only This Fixture***, ***Multiple Fixture***, or ***Other Fixture Type***, and ***Fixture to Fixture***. A list of the updated software files will be displayed.
   
   >* See the separate instructions below for doing a **Fixture to Fixture** software update process.
3. Select the file that needs to be uploaded. The message **"Are you sure?"** will be displayed. Press **< ENTER >**.
   >**If the selected file is incorrect, the upgrade will fail, and the display will go back to the main interface.**
   >**Repeat steps 1-3 using the correct file**.
4. If the selected file is correct, the upgrade will start. DO NOT turn off the power or disconnect the USB during the process. USB update can take several minutes to complete.
5. When the update is complete, the fixture will automatically reboot.
6. Go to Fixture Information on the product’s menu map and confirm the firmware revision.
7. When the boot-up process is finished, restart the product.

### Special Notes
* Place the .chl file in the root directory of the USB drive.
* The product's USB port supports up to 32GB capacity and only works with FAT32 file format.
* Turning off the power or removing the USB while still blinking during the update will cause partial or total firmware failure in the targeted fixture(s). A force upload will be needed to fix firmware failure issues.


&nbsp;  

## Fixture to Fixture Software Update

To update the firmware using a DMX cable connection, follow the instructions below:
1. Power on the products.
2. Connect the DMX out of the STRIKE Array 2C Driver with the latest firmware to the DMX in of the STRIKE Array 2C Driver that needs to be updated.
3. Go to the **Update Firmware** main level of the receiving product.
4. Select the **Fixture to Fixture** option.
5. A warning ***"make sure no other signal, Network, or DMX controller is being sent! and press enter key to start update"*** will show on the display. Press **< ENTER >** to start the update.
   >* DO NOT turn off the power or disconnect the DMX cable during the process. The update can take several minutes to complete.
   >* If the connected product is incorrect or has the incorrect sofware, the upgrade will fail, and the display will go back to the main interface. Repeat **steps 1-5** using a STRIKE Array 2C Driver with valid software.
6. If the connected product is valid, the update will start. DO NOT turn off power or disconnect the DMX cable during the process. The update can take several minutes to complete.
7. When the update is complete, the product will automatically reboot.
8. Go to the **Information** level of the prodduct's main menu and confirm the software update.

### Special Notes
* When updating software using the **Fixture to Fixture** option, make sure no other DMX or Ethernet signals are connected to the products.
* Turning off the power, removing the DMX cable, or not setting the fixture to the correct protocol during the update can cause partial or total firmware failure in the targeted fixture. The user will need an **Upload 03** device to fix the software failure issues. Please contact Chauvet customer service for this device.

&nbsp;

## Force Upload
1.	Link the target fixture to the main fixture via a DMX 5-pin connection. Ensure that the target fixture is turned off.
2.	Turn on the main fixture and set its protocol to DMX512.
3.	Plug the flash drive into the USB-C port of the main fixture.
4.	Go to Upgrade Firmware on the menu map.
5.	Choose between **Multiple Fixture** and **Other Fixture Type**. Press **< ENTER >**.
      * **Multiple Fixture** : Both the target fixture and main fixture are from the same product line (e.g., 2 Color STRIKE M fixtures).
      * **Other Fixture Type**: The target fixture and main fixture are from different product series (e.g., a Color STRIKE M as the target fixture and a Maverick Silens 2 Profile as the main fixture).
6.	Select the file that needs to be uploaded. The message ***“Are you sure?”*** will appear on the screen. Press **< ENTER >**. Turn on the target fixture within 1–2 seconds of pressing **< ENTER >**. The display on the target fixture should remain off.
      a. The main fixture will show the update progress (0–100%).
      b. The target fixture’s display will turn on, and a notification ***“< UPDATE >”*** will appear on the screen.
7.	DO NOT turn off power or remove the USB flash drive. Once the software is done uploading, the target fixture will automatically reboot.
8.	Go to the target fixture’s main menu and confirm that the firmware version has been updated.
9.	Reboot the target fixture.

### Special Notes
* A Force Upload process requires a target fixture (the fixture that needs a Force Upload and a main fixture (the fixture that controls the upload process).
* The Force Upload process can only be done one target fixture at a time.

