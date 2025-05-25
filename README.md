How to Fix SP Flash Tool Errors (BROM Error Codes):
---------------------------------------------------

### SP Flash Tool Failed to enumerate COM Port

This error clearly means that the Flash Tool has issues finding the COM port on which your device is connected.

**Solution**:

1.  Make sure to run SP Flash Tool as administrator on your computer. (A viewer suggested this solution, as it helped him fix the failed to enumerate COM Port issue.)
2.  Connect your watch to another Port and make sure you have USB Drivers installed.
3.  Open "_Device Manager"_ and find the COM port of the device you connected. Once found, open Flash Tool, click on Options -> COM Port -> Select the COM Port on which you have connected your device.

### The device automatically disconnects during flashing

**Meaning**: Device disconnects as soon as the flashing process begins, interrupting the process.

**Solution**:

1.  Try a different USB Cord, USB Port & PC

3.  Hold the Volume Down or Up button while connecting the device to the PC for flashing

### SP Flash Tool remains at 0%

**Solution**:

1.  Install necessary [MediaTek VCOM drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/) on PC.
2.  Use the latest version of SP Flash Tool - [Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)

Follow the troubleshooting guide on how to [fix the Flash tool Stuck at 0% (waiting)](https://www.gizmoadvices.com/fix-sp-flash-tool-stuck-0/) issue.

### Error: Initialize scatter file failed. Please check the scatter file name you load is legal

**Meaning**: SP Flash Tool doesn't accept the name of the scatter file.

**Solution**:

1.  Make sure the scatter file was not renamed.
2.  Try a higher version of SP Flash Tool [\[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]

### Error: USB device not recognized

This error occurs while you connect your device to the PC. It shows a prompt on the system tray after connecting your device.

**Meaning**: PC is having trouble communicating with your device (It occurs due to interruption, hardware, or driver problems).

**Solution**:

1.  Try a different USB Cord, USB Port, or PC.

3.  Install the latest [MediaTek USB drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/) on PC.

### Error: Please select one ROM at least before execution

**Meaning**: SP Flash Tool fails to recognize that there is an item ticked.

**Solution**:

1.  Select the Scatter file again and untick all the items which you don't want to flash one by one. Don't use the checkbox, which un-ticks all the things at once and then checks one by one.

### Error: PRO\_INFO: Failed to get PMT info

**Meaning**: SP Flash Tool is having problems reading the phone.

**Solution**:

1.  Use different PC and USB Cable.

3.  Ensure that the phone is powered off with a charged battery inside when connecting.

**Note**: Some phones require you to remove the battery while flashing. In this case, Solution 1 is the one you should follow.

### Error 1002: S\_INVALID\_ARGUMENTS

**Meaning**: Invalid Scatter file.

**Solution**: Load the correct scatter file.

### Error 1012: BROM ERROR: S\_NOT\_ENOUGH\_MEMORY (1012)

**Meaning**: The version of SP Flash Tool doesn't support the size(s) of the file(s) in the firmware or ROM.

**Solution**:

1.  Use the latest version of Flash Tool \[[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]

### Error 1003: S\_COM\_PORT\_OPEN\_FAIL (1003)

**Meaning**: SP Flash Tool encountered an error while communicating with the device via the target port.

**Solution**:

1.  Connect the device to a different USB Port on the PC
2.  Try different versions of SP Flash Tool \[[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]
3.  Try using different USB Cable
4.  Make sure the device's USB port is not damaged

### Error 1013: BROM ERROR: S\_COM\_PORT\_OPEN Fail (1013)

**Meaning**: SP Flash Tool encountered an error while communicating with the device via the target port.

**Solution**:

1.  Connect the device to a different USB Port on the PC
2.  Try different versions of SP Flash Tool \[[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]
3.  Try using different USB Cable
4.  Make sure the device's USB port is not damaged

### Error 1011: S\_NOT\_ENOUGH\_STORAGE\_SPACE

**Meaning**: The size of any part of the firmware is larger than the allotted space (usually a block or core)

**Solution**:

1.  Change the version of the SP Flash Tool. [Download from here](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).

**Note**: It is learned that this error sometimes occurs on the "raw" versions of the flash tool. So changing the version might help.

### Error 1022:

**Meaning**: The version of the SP Flash tool is not compatible with your device, or the USB interface is not working.

**Solution**:

1.  Use the different or latest version of SP Flash Tool - [Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)
2.  Change USB Cable or USB Port.

### Error 1040: S\_UNSUPPORTED\_OPERATION (1040)

**Meaning**: Flash boot files & Scatter.txt don't match.

**Solution**:

1.  Make sure the correct scatter file is loaded.

### Error 1042: BROM ERROR: S\_TIMEOUT (1042)

**Meaning**: The flashing process took too long, and the SP Flash Tool encountered a timeout.

**Solution**:

1.  Try flashing one file at a time
2.  Use the latest version of SP Flash Tool \[[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]

4.  Use different PC and USB Cable

### Error 2: BROM ERROR: ?? (2)

**Meaning**: SP Flash Tool was unable to communicate with the device.

**Solution**:

1.  Try using a different PC (preferably Windows 7)
2.  Install [MediaTek USB Drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/) on PC

4.  Use another USB Cable

### Error 4008: BROM ERROR : S\_FT\_DOWNLOAD\_FAIL (4008)

**Meaning**: There is an interruption between the SP Flash Tool and the device communication, and the SP Flash Tool encountered an error while flashing files.

**Solution**:

1.  Take out the battery and re-insert it back.
2.  Use different USB Cable, Port, and PC.

4.  Right click flash\_tool.exe -> Properties -> Compatibility -> Set to Windows XP Service Pack 3 -> Apply -> OK -> Run flash\_tool.exe as administrator.
5.  Make sure the battery has enough charge left.

### Error 2004: BROM ERROR : S\_FT\_DOWNLOAD\_FAIL (2004)

**Meaning**: There is an interruption between the SP Flash Tool and the device communication, and the SP Flash Tool encountered an error while flashing files.

**Solution**:

1.  Take out the battery and re-insert it back.
2.  Use different USB Cable, port, and PC.

4.  Right click flash\_tool.exe -> Properties -> Compatibility -> Set to Windows XP Service Pack 3 -> Apply -> OK -> Run flash\_tool.exe as administrator.
5.  Make sure the battery has enough charge left.

### Error 2005: BROM ERROR: S\_BROM\_CMD\_STARTCMD\_FAIL (2005)

**Meaning**: Device attempted to power on before SP Flash Tool could flash the files to it.

**Solution**:

1.  Take out the battery and re-insert it back.
2.  Use different USB Cable, port, and PC.

4.  Right click flash\_tool.exe -> Properties -> Compatibility -> Set to Windows XP Service Pack 3 -> Apply -> OK -> Run flash\_tool.exe as administrator.
5.  Make sure the battery has enough charge left.

### Error 2020: BROM ERROR : S\_BROM\_CHKSUM16\_MEM\_RESULT\_DIFF (2020)

**Meaning**: Flash Tool encountered a problem moving files to be flashed to the device's internal SRAM.

**Solution**:

1.  use the latest version of the SP flash tool \[[Download Here](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]
2.  In SP flash tool, navigate to Options > Option > Connection > Battery. Set it to "with battery".
3.  Use the Format all + Download option
4.  Hold both volume buttons before connecting to the PC for flashing and release once flashing begins

### Error 3001: S\_DA\_EXT\_RAM\_ERROR

The SP Flash Tool Error 3001 occurs due to connection problems. Check the cable and reconnect to another port. If it still occurs, try using a different PC.

### Error 3012: NAND\_FLASH\_NOT\_FOUND

**Meaning**: Problem associated with the definition of flash memory.

**Solution**:

1.  Use the different version of flash tools - [Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)
2.  Use different PC, USB Cable, and USB Port.

### Error 3140: BROM ERROR: S\_DA\_UPDATE\_BOOLOADER\_EXIST\_MAGIC\_NOT\_MATCHED

**Meaning**: SP flash tool encountered an error flashing a selected file to a non-specified partition

**Solution**:

1.  Use the latest version of SP Flash Tool - [Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)

3.  Use format option and then download in SP Flash Tool

### Error 3144: S\_DA\_EMMC\_FLASH\_NOT\_FOUND (3144)

**Meaning**: Flash boot files and scatter mismatch. Note EMMC partition device and MTD partition device use different TXT boot files.

**Solution**:

1.  Choose the correct Scatter file.
2.  Use a different PC (preferably Windows XP) with all the drivers loaded.

### Error 3149: BROM ERROR : S\_DA\_SDMMC\_WRITE\_FAILED (3149)

**Meaning**: SP Flash tool is unable to flash files to the device.

**Solution**:

1.  Use the latest version of the SP flash tool and run it as administrator. \[[Download here](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]

3.  Format first then Download
4.  Don't tick a box with an unspecified/empty file path
5.  Ensure the phone is switched off and has enough charge before connecting to the PC for flashing
6.  Try a different PC
7.  Try a different ROM

9.  Try a different USB cord
10.  Try formatting the phone first before flashing files to it

### Error 3168: BROM ERROR: S\_CHIP\_TYPE\_NOT\_MATCH (3168)

**Meaning**: SP Flash Tool detects that there is a mismatch between the information provided in the scatter file and the device's info.

**Solution**:

1.  Make sure you are using the correct ROM file for your device.

3.  Use the higher version of SP Flash Tool - [Download here](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)
4.  Install correct drivers on PC.

### Error 3182: BROM ERROR: S\_STORAGE\_NOT\_MATCH (3182)

**Meaning**: The firmware you are trying to flash is not compatible with your device.

**Solution**: Try getting the appropriate firmware for your device model.

### Error 3167: BROM\_ERROR: S\_STORAGE\_NOT\_MATCH (3167)

**Meaning**: The firmware you are trying to flash is not compatible with your device.

**Solution**: Try getting the appropriate firmware for your device model.

### Error 3178: BROM\_ERROR: S\_STORAGE\_NOT\_MATCH (3178)

**Meaning**: The firmware you are trying to flash is not compatible with your device.

**Solution**: Try getting the appropriate firmware for your device model.

### Error 4001: S\_FT\_DA\_NO\_RESPONSE or Da didn't send response data to Flash Tool

**Meaning**: SP Flash Tool facing problem communicating with the device.

**Solution**:

1.  Use a different USB Port.
2.  Install [MediaTek VCOM drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/) on PC.
3.  Run Flash\_tool.exe as administrator.
4.  Use a different PC (preferably Windows 7 or XP).

6.  Try different USB Cable.

### Error 4004: Driver Error

**Meaning**: Drivers not found or corrupted.

**Solution**: Uninstall drivers and re-install them.

### Error 4009: S\_FT\_READBACK\_FAIL (4009)

**Meaning**: SP Flash Tool failed to create a Readback file, possibly due to not enough space for a file or file cannot be overwritten because it is locked.

**Solution**:

1.  Use the different version of SP Flash Tool \[[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]
2.  Delete old Readback files

### Error 4010: BROM ERROR : S\_FT\_FORMAT\_FAIL

**Meaning**: The blocks map in the scatter file doesn't match the device's partition sizes

**Solution**:

1.  Use the correct firmware for your device model.

3.  Use the latest version of SP Flash Tool \[[Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]

### Error 4017: BROM ERROR: S\_FT\_NAND\_READLEN\_NOT\_ALIGNMENT (4017)

**Meaning**: You're trying to flash a file that has not been processed for flashing via the SP flash tool

### Error 4032: BROM ERROR : S\_FT\_ENABLE\_DRAM\_FAIL (4032) \[EMI\] Enable DRAM fail

**Meaning**: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings

**Solution**:

1.  Ensure that the firmware you are flashing is made for your device model.
2.  Delete the SP Flash Tool folder and re-extract it.
3.  Ensure you tick the boxes for only the files present in the ROM you're about to flash
4.  Might have the wrong driver installed. Uninstall the VCOM, Preloader, and MTK drivers and re-install them.

### Error 4050: S\_FT\_NEED\_DOWNLOAD\_ALL\_FAIL

**Meaning**: The SP Flash Tool Error Code 4050 occurs when block sizes are not the same in the PMT and scatter. In general, this error is treated to download all the blocks (one can use data enough), then the size in the PMT should switch to the right.

**Solution**:

1.  Use a different version of Flash Tool - [Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)

### Error 4058: BROM ERROR: S\_FT\_GET\_MEMORY\_FAIL (4058)

**Meaning**: Flash tool was unable to locate the partition you're trying to flash.

**Solution**: Un-tick any item with a blank or empty location

### Error 5002: S\_INVALID\_DA\_FILE

**Meaning**: The Download Agent (DA) file selected is not compatible. DA file is attached to the Flash Tool release, so choose the one which is provided in the Flash Tool folder.

**Solution**:

1.  Choose the DA file from the SP Flash Tool folder.

### Error 5007: BROM ERROR : S\_FTHND\_FILE\_IS\_NOT\_LOADED\_YET (5007)

**Meaning**: You're trying to flash a file with the unspecified path (no file selected in the item box)

**Solution**:

1.  Make sure the scatter file is in the same folder where the other files to be flashed are located.
2.  Untick any item whose file you do not have or whose path is not specified.

### Error 5054: BROM ERROR S\_DL\_GET\_DRAM\_SETTINGS\_FAIL (5054)

**Meaning**: The files you are trying to flash are not compatible with the device.

**Solution**:

1.  Ensure you are using the correct files.

### Error 5069: BROM ERROR : S\_DL\_PMT\_ERR\_NO\_SPACE (5069)

**Meaning**: The size of a file is larger than the available partition size.

**Solution**:

1.  Ensure that you are flashing the correct files to the device.
2.  Try another ROM.

### Error 5056: BROM ERROR : S\_DL\_PMT\_ERR\_NO\_SPACE (5056)

**Meaning**: The size of a file is larger than the available partition size.

**Solution**:

1.  Ensure that you are flashing the correct files to the device.
2.  Try another ROM.

### Error 5066: S\_DL\_PC\_BL\_INVALID\_GFH\_FILE\_INFOR

**Meaning**: Wrong files. The Scatter file of the chosen folder is not yet prepared for the FT files.

**Solution**:

1.  Choose the correct scatter file prepared for the FT files.

### Error 5095: S\_DL\_MAUI\_FLASH\_ID\_NOT\_MATCHED\_WITH\_TARGET (5095)

**Meaning**: When you choose the wrong file, for example, another type of flash downloads into the current flash, the tool will warn with this message. The chosen flash files are not compatible with your device.

### Error 6010: BROM ERROR: SP FLASHTOOL ERROR 6010 CODE DOWNLOAD FORBIDDEN

**Meaning**: The device has a protected or locked bootloader.

**Solution**: Unlock the bootloader on your device.

### Error 6012: BROM ERROR: S\_SECURITY\_SF\_CODE\_COMMAND\_FORBIDDEN (6012), MSP ERROR CODE: 0X00

**Meaning**: The Download-Agent being used is incompatible with the device.

**Solution**: Set Download-Agent to MTK\_AllInOne\_DA.bin

### Error 6047: BROM ERROR: S\_SECURITY\_SECURE\_USB\_DL\_IMAGE\_HASH\_FAIL

**Meaning**: Hash (integrity) check of the files being flashed failed.

**Solution**:

1.  Use SP Flash Tool V5.1516.00 from [here](https://getspflashtool.com/windows/sp-flash-tool-v5-1516/)
2.  Select the right Download Agent file
3.  Navigate to Options > Option > Download and untick DA DLL All…

### Error 6124: BROM ERROR: S\_SECURITY\_INVALID\_PROJECT (6124), MSO ERROR CODE: 0X00

**Meaning**: Wrong flash settings or firmware.

**Solution**:

1.  Use the correct firmware for your exact device model

3.  Select the correct Download Agent file in the SP flash tool
4.  Go to Options > Option > Connection > USB Speed > Full Speed
5.  Go to Options > Option > Download > Untick DA DL All with Checksum

### Error 8038: Error 8038! Android download pmt is ready, and layout has been changed / PMT changed for the ROM

**Meaning**: SP Flash Tool is having trouble writing to certain partitions due to some incompatibility.

**Solution**:

1.  Format the phone in the SP flash tool (Do not format bootloader) then try flashing the files again using Download
2.  If Download doesn't work then do a firmware upgrade
3.  If the MTK backup contains more than one scatter file, retry flashing with the other scatter file.
4.  If that isn't feasible, try formatting first or use the firmware upgrade

6.  If that doesn't work, open the scatter file using Notepad++ and change \_\_NODL\_FAT to FAT by removing "\_\_NODL\_".

### Error 8100:

**Meaning**: Cannot find the USB port.

**Solution**:

1.  Install the Drivers. If already installed, uninstall them and re-install them again.

### Error 8200:

**Meaning**: Invalid file or incompatible recovery file.

**Solution**:

1.  Find the right recovery file.
2.  Use the latest version of the SP Flash Tool. \[[Download Here](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool)\]

### Error 8406: SP FLASH TOOL ERROR (8406)

**Meaning**: Compatibility issues.

**Solution**:

1.  Flash the right firmware for your exact device model.
2.  Update VCOM drivers.

### Error 8417: BROM ERROR: Initialize scatter file failed. Please check the scatter file name you load is legal

**Meaning**: The format of the Scatter file is invalid.

**Solution**:

Open the scatter file in Notepad++, the first line must beginning with:

############################################################################################################## General Setting #

If there is anything else above this then delete it and save the scatter file.

### Stuck at Download DA 100%

**Meaning**: SP Flash Tool is having trouble communicating with your device.

**Solution**:

1.  Uninstall and re-install [MediaTek drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/).

### SP Flash Tool flashing process was successful, but the phone's calibration doesn't work

If, after flashing the files using SP Flash Tool soft keys and touch doesn't work or respond, follow the below solution.

**Solution**:

Edit the scatter file using Notepad++ and remove the NODL\_ (or set is\_download: false to is\_download: true) in front of the items you have in the backup folder but aren't listed when you load the scatter file in the SP flash tool. Removing NODL\_ or setting is\_download to true makes the item listed/available in the SP flash tool when you load the scatter file after saving it.

### USB device not recognized

**Meaning**: The PC is having trouble communicating with your device because of interruption, hardware, or driver problem.

**Solution**:

1.  Remove and install the [MediaTek MTK drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/) again on your PC.

3.  Try a different USB cable.
4.  Connect the device to a different USB Port.
5.  If the above solutions don't work, try using another PC.

### Error 0xFDA: BROM ERROR: S\_FT\_GET\_MEMORY\_FAIL (0xFDA)

**Meaning**: SP Flash Tool encountered an error reading your device’s storage.

**Solution**:

1.  Try a different USB cable.
2.  Connect the device to a different USB Port.
3.  If the above solutions don't work, try using another PC.

### Error 0x13BE: S\_DL\_GET\_DRAM\_SETTING\_FAIL (0x13BE)

**Meaning**: The firmware you are trying to flash is either not compatible or you have selected the wrong flashing settings.

**Solution**:

1.  Make sure that the firmware you are trying to flash is actually for your device model.
2.  Only tick the boxes only for the files which are available in the ROM folder you're trying to flash.

### Error 0x3: BROM ERROR:?? (0x3)

**Meaning**: SP flash tool encountered an error maintaining the connection with the device during the flashing process.

**Solution**:

1.  Uninstall and re-install MTK VCOM drivers on your PC.
2.  Try a different USB cable.

4.  Connect the device to a different USB Port.
5.  If the above solutions don't work, try using another PC.

### Error 0x7D4: BROM ERROR: S\_BROM\_DOWNLOAD\_DA\_FAIL (0x7D4)

**Meaning**: SP Flash Tool encountered an error writing to the device.

**Solution**:

1.  Try changing the Download Agent (Secure Boot DA) file.

3.  Use the latest version of SP Flash Tool – [Download here](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).
4.  Make sure that your device's battery is sufficiently charged.
5.  Make sure the device's USB port is not damaged.
6.  Ensure that the file names match what's in the scatter file.
7.  Try a different USB cable.
8.  Connect the device to a different USB Port.

10.  If the above solutions don't work, try using another PC.

### Error 0x8: BROM ERROR:?? (0x8)

**Meaning**: The size of the file you are trying to flash is larger than the partition size.

**Solution**:

1.  Ensure that the files you're trying to flash are actually for your device's exact model.
2.  Try another Stock ROM.
3.  Change the phone's EMMC chip.

5.  Try using a different PC.

### Error OXFC0: BROM ERROR S\_FT\_ENABLE\_DRAM\_FAIL (OXFC0)

**Meaning**: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings.

**Solution**:

1.  Ensure that the files you're trying to flash are actually for your device's exact model.

3.  Only tick the boxes only for the files which are available in the ROM you're trying to flash.
4.  Uninstall the VCOM, Preloader, and MTK drivers and re-install them on your PC.
5.  Use the latest version of the [Smartphone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).
6.  Delete the SP Flash Tool folder and re-extract it.

8.  Ensure that the phone is powered off (with the battery inserted) before connecting to the PC for flashing.
9.  If the above solution doesn't work, then you can try holding down the Volume Down button and connect the phone to the PC. You can also try holding Volume UP, Power and Volume Down, Power, and Volume UP buttons.

11.  Format the phone from Settings before trying to flash the files again.

### Error 0X411: BROM ERROR: S\_CHKSUM\_ERROR (0X411)

**Meaning**: There was a checksum error when flashing the firmware.

**Solution**:

1.  Delete any file with the checksum in its name from the ROM/firmware folder.
2.  Go to Options > Option > Download > Un-tick DA DL all with checksum.

### Error 0xFA1: BROM ERROR: S\_FT\_DA\_NO\_RESPONSE (0xFA1)

**Meaning**: SP flash tool encountered an error communicating with the device.

**Solution**:

1.  Install MTK VCOM drivers on your PC. If already installed, uninstall and re-install them.
2.  Ensure that the device is powered off and has charged battery inserted.
3.  Do not hold any button when connecting the device to the PC for flashing.

5.  Try a different USB cable.
6.  Connect the device to a different USB Port.

8.  If the above solutions don't work, try using another PC.

### TOOL DL image Fail!

**Meaning**: DA DL all with the Checksum option, is disabled in the SP flash tool.

**Solution**:

1.  In SP Flash Tool, navigate to Options > Option > Download > Tick DA DL all with checksum and re-flash the firmware.

### Error 0xFC0: BROM ERROR: S\_FT\_ENABLE\_DRAM\_FAIL (0xFC0)

**Meaning**: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings.

**Solution**:

1.  Ensure that the files you're trying to flash are actually for your device's exact model.
2.  Only tick the boxes only for the files which are available in the ROM you're trying to flash.
3.  Uninstall the VCOM, Preloader, and MTK drivers and re-install them on your PC.
4.  Use the latest version of the [Smartphone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).

6.  Delete the SP Flash Tool folder and re-extract it.
7.  Ensure that the phone is powered off (with the battery inserted) before connecting to the PC for flashing.

9.  If the above solution doesn't work, then you can try holding down the Volume Down button and connect the phone to the PC. You can also try holding Volume UP, Power and Volume Down, Power, and Volume UP buttons.
10.  Format the phone from Settings before trying to flash the files again.

### Error 0xC0050003: BROM ERROR: STATUS\_DOWNLOAD\_EXCEPTION (0xC0050003)

**Meaning**: SP flash tool encountered an error writing to one or more partitions.

**Solution**:

1.  [Download](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool) the latest version of the Smart Phone Flash Tool and re-flash the firmware.

3.  Try flashing one partition at a time to figure out which partition is resulting in the error.
4.  Try a different USB cable.
5.  Connect the device to a different USB Port.

7.  If the above solutions don't work, try using another PC.

### Error 0xc002002A: BROM ERROR: STATUS\_SEC\_IMG\_TYPE\_MISMATCH (0xc002002A)

**Meaning**: The firmware you're trying to flash is either not compatible with your device, or you have selected the wrong flashing settings or verified boot is enabled.

**Solution**:

1.  Unlock the bootloader before flashing the firmware.
2.  Ensure that the files you're trying to flash are actually for your device's exact model.

4.  Only tick the boxes only for the files which are available in the ROM you're trying to flash.
5.  Uninstall the VCOM, Preloader, and MTK drivers and re-install them on your PC.
6.  Use the latest version of the [Smartphone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).

8.  Delete the SP Flash Tool folder and re-extract it.
9.  Ensure that the phone is switched off (with the battery inserted) before connecting to the PC for flashing.
10.  If the above solution doesn't work, then you can try holding down the Volume Down button and connect the phone to the PC. You can also try holding Volume UP, Power and Volume Down, Power, and Volume UP buttons.

12.  Format the phone from Settings before trying to flash the files again.

### Error 0XFA8: BROM ERROR: S\_FT\_DOWNLOAD\_FAIL (0XFA8)

**Meaning**: SP flash tool encountered an error while attempting to flash the firmware.

**Solution**:

1.  Make sure that the device is switched off, and the battery is in the device before connecting for flashing.
2.  Use the format option and then download it in the SP flash tool.

4.  Try changing the Download Agent setting in Smartphone Flash Tool.
5.  Try a different USB cable.

7.  Try connecting the device to a different USB Port.
8.  Try using a different PC.

### Error 0x7D5: BROM ERROR: S\_BROM\_CMD\_STARTCMD\_FAIL (0x7D5)

**Meaning**: The device attempted to power on before the SP flash tool could flash the files to it.

**Solution**:

1.  Make sure the battery is sufficiently charged on your device.

3.  Take out and re-insert the battery.
4.  Try using a different USB cable or COM port or PC.

6.  Right click flash\_tool.exe -> Properties -> Compatibility -> Set to Windows XP Service Pack 3 -> Apply -> OK -> Run flash\_tool.exe as administrator.
7.  Do not hold any button when connecting to the PC.

### Error: Boundary Check Failed: rom\_end\_addr >= next rom begin\_addr.

**Meaning**: The firmware has a partition that wasn't included while backing up the firmware. SP Flash Tool encountered an error in the end address of the preloader partition and the begin address of the PGPT partition (i.e., the partition which wasn't included in the backup).

**Solution**:

1.  Close the error message and manually select the location of all the files in the scatter file from the bottom to the top. Meaning that a preloader would be the last thing you will select.

3.  If that doesn't work, open and modify the scatter file using Notepad++ then change the "boundary\_check: True" to "boundary\_check: False".

### Error 3179: BROM ERROR: S\_CHIP\_TYPE\_NOT\_MATCH (3179)

**Meaning**: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings.

**Solution**:

1.  Ensure that the files you're trying to flash are actually for your device's exact model.
2.  Only tick the boxes only for the files which are available in the ROM you're trying to flash.

4.  Uninstall the VCOM, Preloader, and MTK drivers and re-install them on your PC.
5.  Use the latest version of the [Smartphone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).
6.  Delete the SP Flash Tool folder and re-extract it.
7.  Ensure that the phone is powered off (with the battery inserted) before connecting to the PC for flashing.
8.  If the above solution doesn't work, then you can try holding down the Volume Down button and connect the phone to the PC. You can also try holding Volume UP, Power and Volume Down, Power, and Volume UP buttons.
9.  Format the phone from Settings before trying to flash the files again.

### Error 5073: BROM ERROR: S\_DL\_READ\_PT\_FAIL (5073)

**Meaning**: Smartphone flash tool encountered an error while trying to format the device.

**Solution**:

*   Use "download only" under the download tab to flash the firmware, and then you can format the device if needed.

### SP Flash Tool force-closes when scatter file is loaded

**Meaning**: SP Flash Tool doesn't support the scatter file because of its blocks or configuration.

**Solution**:

*   Open the scatter file using Notepad++ and locate the last partition on the list (flashinfo) and change the is\_download: true to is\_download: false. Once done, save the scatter file and reload it in SP Flash Tool.

### Storage type mismatch!

**Message**:

scatter storage type is HW\_STORAGE\_EMMC

target storage type is HW\_STORAGE\_NAND

(or)

scatter storage type is HW\_STORAGE\_EMMC

target storage type is HW\_STORAGE\_NONE

**Meaning**: There is a mismatch between the device's storage type and that which the scatter file expects.

**Solution**:

1.  Try using a different firmware or ROM.

3.  Try using SP Flash Tool version 3.x. If it doesn't work, try using different versions and make sure to run it as administrator.

### Error 8045: No Valid Partition Management Table (PMT) for storage

**Meaning**: SP Flash Tool failed to identify the device's partition ahead of the file writes.

**Solution**:

*   Try flashing the firmware using Download only.

### Error 1041: BROM ERROR: S\_CHKSUM\_ERROR (1041)

**Meaning**: There was a checksum error when flashing the firmware.

**Solution**:

1.  Delete any file with the checksum in its name from the ROM/firmware folder.
2.  Go to Options > Option > Download > Un-tick DA DL all with checksum.

### Error 6126: BROM ERROR: S\_SECURITY\_SECRO\_HASH\_INCORRECT (6126), MSP ERROE CODE: 0x00

**Meaning**: The ROM contains a checksum file, but DA DL All With CheckSum is un-checked.

**Solution**:

*   Tick DA DL All With Check Sum under Options > Option > Download.

### Error 6128: BROM ERROR: S\_SECURITY\_AC\_REGION\_NOT\_FOUND\_IN\_SECROIMG (6128), MSP ERROR CODE: 0X00

**Meaning**: The ROM contains a checksum file, but DA DL All With CheckSum is un-checked.

**Solution**:

*   Tick DA DL All With Check Sum under Options > Option > Download.

### Error 0xC0050005: ERROR STATUS\_EXT\_RAM\_EXCEPTION (0xC0050005)

**Meaning**: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings.

**Solution**:

1.  Ensure that the files you're trying to flash are actually for your device's exact model.

3.  Only tick the boxes only for the files which are available in the ROM you're trying to flash.
4.  Make sure your device's battery is sufficiently charged.

### Error (3): BROM ERROR:?? (3)

**Meaning**: There is a problem with the format of the scatter file or files being flashed. Example – trying to flash .bin files using SP Flash Tool.

**Solution**:

*   Check the scatter file and firmware files you are trying to flash to make sure that they're not meant to be flashed using a different tool.

### Error 6104: BROM ERROR: S\_SECURITY\_SECURE\_USB\_DL\_DA\_RETURN\_INVALID\_TYPE (6104), MSP ERROR CODE: 0X00

**Meaning**: Wrong flash settings or firmware/ROM files.

**Solution**:

1.  Make sure you have selected the correct Download Agent file in SP Flash Tool and are using the firmware meant for your device's exact model.
2.  Go to Options > Option > Connection > USB Speed > Full Speed.
3.  Go to Options > Option > Download > un-tick DA DL ALL with Checksum.

### Error 3183: BROM ERROR: S\_CHIP\_TYRE\_NOT\_MATCH (3183)

**Meaning**: SP Flash Tool believes that there is a mismatch between the information provided in the scatter file and device info.

**Solution**:

1.  Make sure to use the ROM/firmware for the exact device model.
2.  Try using the higher version of the SP Flash Tool.
3.  Uninstall and re-install the [MediaTek MTK USB Drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/) on your PC.

### Error 0xC0060001: BROM ERROR: S\_BROM\_CMD\_STARTCMD\_FAIL (0xC0060001)

**Meaning**: The device attempted to power on before the SP flash tool could flash the files to it.

**Solution**:

1.  The device might require a custom Download Agent (DA) to be flashed.
2.  Make sure the battery is sufficiently charged before flashing.
3.  Take out and re-insert the battery.
4.  Try using a different USB cable or COM port or PC.
5.  Right click flash\_tool.exe -> Properties -> Compatibility -> Set to Windows XP Service Pack 3 -> Apply -> OK -> Run flash\_tool.exe as administrator.
6.  Do not hold any button when connecting to the PC.

### Error: PMT changed for the ROM; it must be downloaded

**Meaning**: The partition table about to be written (from the scatter file) is different from the device's current partition table layout.

**Solution**:

1.  Ensure that the scatter file and firmware/ROM files you're trying to flash are for your device's exact model.
2.  If you're trying to flash only a few files from the firmware, then you need to get the firmware to complement and then flash using download only.
3.  If you're trying to flash the complete firmware, then try using the "Firmware Upgrade" option or Format first before the "download only" option.

### Error 6004: ERROR: S\_SECURITY\_SLA\_FAIL (6004), MSP ERROE CODE: 0X00

**Meaning**: The Download Agent file isn't compatible with the device.

**Solution**:

1.  Try using a different Download Agent file.
2.  Try using a different version of the [Smartphone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).
3.  Ensure you are using the right Authentication file.

### Error 6045: S\_SECURITY\_SECURE\_USB\_DL\_IMAGE\_SIGN\_HEADER\_NOT\_FOUND (6045), MSP ERROE CODE: 0x00

**Meaning**: The image files you are trying to flash do not contain –sign header.

**Solution**:

1.  Use the SP Flash Tool v5.1532.00 – [Download here](https://getspflashtool.com/windows/sp-flash-tool-v5-1532/).
2.  Load the Auth file for the device in the flash tool.

4.  Try flashing a factory-signed firmware.
5.  Flash the unsigned image using the 'Write Memory' tab in SP Flash Tool. To activate the write memory tab, press 'Ctrl + Alt + V' to enable advanced mode and then click Window > Write Memory.

### Error 2035: BROM ERROR: S\_BROM\_CMD\_JUMP\_DA\_FAIL (2035)

**Meaning**: SP Flash Tool encountered an error connecting to the device.

**Solution**:

1.  Ensure that the battery is inserted, and you're not holding any button when connecting the device to a PC for flashing.
2.  Uninstall and re-install the [MediaTek MTK VCOM Drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/).
3.  Disable any modem manager or software which might be blocking ports on the PC.

5.  Linux / Ubuntu users, make sure you installed 'libusb-dev' then blacklist Ubuntu's modem manager (because it controls port /dev/ttyACM0, which is causing SP Flash Tool from running properly).

### Error 0x412: BROM ERROR: S\_TIMEOUT (0X412)

**Meaning**: SP Flash Tool encountered a timeout when trying to flash, i.e., flashing took long to start or complete.

**Solution**:

1.  Make sure that files are loaded in SP Flash Tool with a valid location. The location should not be empty.
2.  Try flashing one file at a time.
3.  Try using a higher version of the [Smart Phone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).

5.  Un-tick larger files or find smaller alternatives.

### Error 6029: S\_SECURITY\_SEND\_AUTH\_FAIL (6029), MSP ERROE CODE: 0x00

**Meaning**: SP Flash Tool failed to authenticate the files you are trying to flash.

**Solution**:

1.  Try another ROM/firmware from a different source.
2.  Get an Auth file for your device model.
3.  For Tecno, Infinix, and Itel devices, use Software Download Tool (Format + Download).

### Error 0x93AF: ROM \[logo\] checksum mismatch checksum\_config\[0x93af\], checksum\_val\[0x94ae\]

**Meaning**: The SP Flash Tool Error Code 0x93AF means that the tool encountered a checksum error.

**Solution**:

1.  Open the checksum file using Notepad++ and search for 0x93af and replace it with 0x94ae.

3.  Delete any checksum file from the ROM/firmware files.

### Error 5011: S\_DL\_SCAT\_INCORRECT\_FORMAT (5011)

**Meaning**: The scatter file has an incorrect format. It has been badly created or modified.

**Solution**:

1.  Download a different scatter file that doesn't throw an error in SPFT. Now open the two scatter files using Notepad++, and you will notice that the incorrect scatter file has the items slightly shifted to the left. Edit the incorrect scatter file to the same format as in the working scatter file.
2.  After modifying the scatter file using the above method, use the latest version of SP Flash Tool e.g., SP Flash Tool v5.1728.
3.  Download another ROM/firmware from a different source.

### Error 0xC52: BROM ERROR: S\_DA\_SDMMC\_WRITE\_FAILED (0XC52)

**Meaning**: SP Flash Tool was unable to flash files to the device.

**Solution**:

1.  Make sure to use the latest version of the SP Flash Tool and run it as administrator.
2.  Format first then Download.
3.  Un-tick the box with an unspecified/empty file path.
4.  Ensure that the battery is sufficiently charged and the device is switched off before connecting to the PC for flashing.
5.  Try a different ROM from a different source.
6.  Try formatting the device first before flashing the files.

8.  Try a different USB cable.
9.  Connect the device to a different USB Port.
10.  If the above solutions don't work, try using another PC.

### Error 0XFAA: BROM ERROR: S\_FT\_FORMAT\_FAIL (0XFAA)

**Meaning**: The source (firmware) doesn’t properly match with the target (phone).

**Solution**:

1.  Try using a different firmware for your device model.
2.  Ensure you're using the right tool for flashing the firmware.

### Error 5072: ERROR: S\_DL\_WRITE\_PT\_FAIL (5072)

**Meaning**: SPFT encountered a problem writing to one or more partitions.

**Solution**:

1.  Make sure the device is powered off with a charged battery inside before connecting to the PC for flashing.
2.  Don't hold any buttons when connecting to the PC.

4.  Try a different USB cable.
5.  Connect the device to a different USB Port.
6.  If the above solutions don't work, try using another PC.

### Error 0xC0070004: ERROR: STATUS\_DA\_HASH\_MISMATCH (0xC0070004)

**Meaning**: Hash (integrity) check for the images being flashed is failed.

**Solution**:

1.  Use SP Flash Tool v5.1516.00 – [Download from here](https://getspflashtool.com/windows/sp-flash-tool-v5-1516/).
2.  Make sure to select the correct Download Agent file.
3.  Navigate to Options > Option > Download > Un-tick DA DL all with checksum.

### Error 6046: BROM ERROR: S\_SECURITY\_USB\_DL\_IMAGE\_SIGNATURE\_VERIFY\_FAIL (6064), MSP ERROR CODE: 0X0

**Meaning**: The SP Flash Tool Error Code 6046 refers to the failed signature verification for the firmware files.

**Solution**:

1.  Select MTK\_AllInOne\_DA.bin as Download Agent file.

3.  Navigate to Options > Option > Download > Un-tick DA DL all with Checksum.

5.  Delete any checksum file in the ROM/firmware folder.

### Error 0XC0060003: ERROR: STATUS\_BROM\_CMD\_SEND\_DA\_FAIL (0XC0060003)

**Meaning**: Smart Phone Flash Tool is unable to read or write to the device using the selected Download Agent.

**Solution**:

1.  The device might require a custom Download Agent (DA) to be flashed.
2.  Make sure the battery is sufficiently charged before flashing.
3.  Take out and re-insert the battery.

5.  Try using a different USB cable or COM port or PC.
6.  Right click flash\_tool.exe -> Properties -> Compatibility -> Set to Windows XP Service Pack 3 -> Apply -> OK -> Run flash\_tool.exe as administrator.

8.  Do not hold any button when connecting to the PC.

### Error 0x94010000: CHIP TYPE NOT match! target refuse value: 0x94010000

**Meaning**: The device likely has a locked/encrypted preloader.

**Solution**:

*   Un-tick preloader when flashing in SP Flash Tool.

### Error 0xC0020029: BROM ERROR: STATUS\_SEC\_IMGHDR\_TYPE\_MISMATCH (0xC0020029)

**Meaning**: You are trying to flash the modified files to a device that accepts only signed or verified images.

**Solution**:

1.  Download and flash the official firmware for your device (usually have –verified or –signed prefixes in their filename).

3.  If possible, unlock the bootloader of your device and then try re-flashing.

### Error 5000: BROM ERROR: S\_AUTH\_HANDLE\_IS\_NOT\_READY (5000)

**Meaning**: The device has a secure boot/bootloader.

**Solution**:

1.  You will need an Auth (\*.auth) file or custom Download Agent (DA) file for the device to proceed with flashing using SP Flash Tool.
2.  For Tecno, Infinix, and Itel devices, use Software Download Tool (Format + Download).

### Error 0xC002002C: ERROR: STATUS\_SEC\_IMG\_HASH\_VFY\_FAIL (0xC002002C)

**Meaning**: The device has a verified boot.

**Solution**:

*   Download and flash the official firmware for your device (usually have –verified or –signed prefixes in their filename).

### Error 0xC0030012: ERROR: STATUS\_SEC\_AUTH\_FILE\_NEEDED (0xC0030012)

**Meaning**: The device has a secure boot.

**Solution**:

*   You will need an Auth (\*.auth) file or custom Download Agent (DA) file for the device to proceed with flashing using SP Flash Tool.

### Error 0xC0060005: ERROR: STATUS\_BROM\_CMD\_FAIL (0xC0060005)

**Meaning**: The device attempted to power on before the SP Flash Tool could flash files to it.

**Solution**:

*   You will need a custom Download Agent (DA) file for your device model.

### Error 8: ERROR: ?? (8)

**Meaning**: The size of a file is larger than the available partition size.

**Solution**:

1.  Make sure that the firmware files you are trying to flash are actually for your device's exact model.

3.  Try another Stock ROM from a different source.
4.  Change the device's EMMC chip.
5.  Try using a different PC.

### Error 0xC0030001: Error: STATUS\_SCATTER\_FILE\_INVALID (0xC0030001)

**Meaning**: SP Flash Tool cannot recognize the scatter file or the location of the scatter file.

**Solution**:

1.  Rename the folder location of the scatter file, including the parent folders too, and remove all special characters / non-English characters from the folder name.
2.  If that doesn't work, then create a new folder on your desktop and copy ONLY the firmware files to the new folder and then retry flashing the contents from the new folder.

### Error: Partition\[nvram\] should NOT set "is\_download" to true in scatter file

**Meaning**: The scatter file specifies to download NVRAM but doesn't specify a file name for NVRAM. This error is common in later versions of the SP Flash Tool.

**Solution**:

1.  Modify the scatter file using notepad++ and add a file name for the NVRAM partition. e.g., "file\_name: nvram.bin" then save and ensure there's a nvram.bin file in the same folder as the scatter file.
2.  If that doesn't work, modify the scatter file using notepad++ and set "is\_download: false" for the NVRAM partition.

### Error 0xC0050001: ERROR: STATUS\_DEVICE\_CTRL\_EXCEPTION (0XC0050001)

**Meaning**: The firmware you are trying to flash is either not compatible or you have selected the wrong flashing settings.

**Solution**:

1.  Make sure that the firmware you are trying to flash is actually for your device model.

3.  Only tick the boxes only for the files which are available in the ROM folder you're trying to flash.
4.  Uninstall and re-install [MediaTek Preloader VCOM USB Drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/).

### Error 0xC002001B: ERROR: STATUS\_SEC\_PUBK\_AUTH\_MISMATCH\_N (0xC002001B)

**Meaning**: The device has a verified boot.

**Solution**:

*   Download and flash the official firmware for your device (usually have –verified or –signed prefixes in their filename).

### Error 5014: ERROR: S\_DL\_SCAT\_ADDR\_IS\_NOT\_ASCENDING\_ORDER (5014)

**Meaning**: The scatter file was badly created or modified, depending on how you obtained the scatter file.

**Solution**:

*   Input the correct values for all "physical\_start\_addr" in the scatter file. The exact value for "physical\_start\_addr" is the same as the value of "linear\_start\_addr".

### Error 0x7F3: BROM ERROR: S\_BROM\_CMD\_JUMP\_DA\_FAIL

**Meaning**: SP Flash Tool is having trouble communicating with the device.

**Solution**:

1.  Ensure that the battery is inserted, and you're not holding any button when connecting the device to a PC for flashing.
2.  Uninstall and re-install the [MediaTek Preloader Drivers](https://www.gizmoadvices.com/mt65xx-preloader-vcom-driver/).

4.  Disable any modem manager or software which might be blocking ports on the PC.

6.  Linux / Ubuntu users, make sure you installed 'libusb-dev' then blacklist Ubuntu's modem manager (because it controls port /dev/ttyACM0, which is causing SP Flash Tool from running properly).

### Error 3154: BROM ERROR: S\_DA\_SDMMC\_WRITE\_FAILED (3154)

**Meaning**: SP Flash Tool Error Code 3154 means that the flash tool is having trouble flashing files to the device.

**Solution**:

1.  Make sure to use the latest version of the SP Flash Tool and run it as administrator.
2.  Format first then Download.
3.  Un-tick the box with an unspecified/empty file path.
4.  Ensure that the battery is sufficiently charged and the device is switched off before connecting to the PC for flashing.

6.  Try a different ROM from a different source.

8.  Try formatting the device first before flashing the files.
9.  Try a different USB cable.
10.  Connect the device to a different USB Port.
11.  If the above solutions don't work, try using another PC.

### Error 0xC0010005: BROM ERROR: STATUS\_PROTOCOL\_ERR (0xC0010005)

**Meaning**: SP flash tool is having trouble communicating with the device.

**Solution**:

*   Make sure that the phone is switched off with the battery inserted before connecting to the PC for flashing.

### Error 0xC0010007: BROM ERROR: INSUFFICIENT\_BUFFER (0xC0010007)

**Meaning**: SP Flash Tool seems to be blocked from flashing files to the device.

**Solution**:

*   If you can boot your device into Fastboot Mode, then unlock the bootloader and then try flashing again.
*   Un-tick OEM and then retry flashing.

### Error 0xC0050007: ERROR: STATUS\_READ\_DATA\_EXCEPTION (0xC0050007)

**Meaning**: SP Flash Tool is unable to readback from the connected device. This error usually occurs, especially when the readback length is too large.

**Solution**:

1.  Download and install updated MTK drivers on your PC.
2.  If you're performing a readback, try skipping cache and userdata.

### Error 0x13CD: BROM ERROR: S\_DL\_PMT\_ERR\_NO\_SPACE (5069)

**Meaning**: The size of a file is larger than the available partition size.

**Solution**:

1.  Make sure that the firmware files you are trying to flash are actually for your device's exact model.
2.  Try another Stock ROM from a different source.

4.  Change the device's EMMC chip.

### Error: LIB DA not match, please re-select DA or ask for help

**Meaning**: SP Flash Tool is having trouble using the selected Download Agent (DA) file.

**Solution**:

1.  Un-tick "Check LIB DA match" from the SP Flash Tool general settings (Options > Option).
2.  Try another version of the SP Flash Tool.

### Error -1073283068: BROM ERROR: STATUS\_DA\_HASH\_MISMATCH (-1073283068), MSP ERROE CODE: 0X00

**Meaning**: The Download Agent (DA) file selected isn't compatible.

**Solution**:

*   Try using Download Agent (DA) + Auth file + Factory ROM.

### Error 0XC50: S\_DA\_SDMMC\_CONFIG\_FAILED (0XC50)

**Meaning**: The device likely has a protected preloader or bootloader.

**Solution**:

*   Un-tick preloader when flashing in SP Flash Tool.

### Error 3152: S\_DA\_SDMMC\_CONFIG\_FAILED (3152)

**Meaning**: The device likely has a protected preloader or bootloader.

**Solution**:

*   Un-tick preloader when flashing in SP Flash Tool.

### Error 0xC0020006: ERROR: STATUS\_SEC\_PL\_VFY\_FAIL (0xC0020006)

**Meaning**: The device likely has a protected preloader or bootloader.

**Solution**:

1.  Try using a signed ROM/firmware.
2.  Try unlocking the bootloader before flashing.

### Error 0xC0030003: ERROR: STATUS\_DA\_SELECTION\_ERR (0xC0030003)

**Meaning**: The Download Agent (DA) file selected is incompatible.

**Solution**:

1.  Try using a different Download Agent file.
2.  Try using Download Agent (DA) + Auth file + Factory ROM.
3.  Try using a different version of the [Smartphone Flash Tool](https://www.gizmoadvices.com/list-sp-flash-tool-error-codes-solution-fix/#where_to_download_SP_Flash_Tool).
4.  For Tecno, Infinix, and Itel devices, use Software Download Tool.

### Error 0xC0030008: ERROR: STATUS\_INVALID\_GPT (0xC0030008)

**Meaning**: EMMC chip is faulty on the device.

**Solution**:

*   Change the device's EMMC chip.

### Error 0xC0050004: ERROR: STATUS\_UPLOAD\_EXCEPTION (0xC0050004)

**Meaning**: SP Flash Tool is unable to communicate with the device.

**Solution**:

1.  Try flashing with/without the battery inserted.
2.  Try a different USB cable.

4.  Connect the device to a different USB Port.
5.  If the above solutions don't work, try using another PC.

### Error 0x1: ERROR: ?? (0x1)

**Meaning**: SP flash tool is having trouble communicating with the device.

**Solution**:

*   Try using a custom Download Agent (DA) and Auth file for your device model.

### Error 0xC0030004: ERROR: STATUS\_PRELOADER\_INVALID 0xC0030004

**Meaning**: There is a problem with the preloader partition name in the scatter file or the flash tool is having trouble communicating with the device.

**Solution**:

1.  Modify the scatter file using Notepad++ and change the partition name to all lower cases. Ex: PRELOADER to preloader or to match the exact file name in the firmware and save the scatter file.
2.  Try holding the volume up or volume down button before connecting the phone to the PC.

4.  If you get an error while trying to format, return to the download tab and tick the checkbox for the preloader, then return to the format tab and retry formatting.

### Error 1003: ERROR: S\_INVALID\_BBCHIP\_TYPE (1003)

**Meaning**: There is a problem with the scatter file.

**Solution**:

*   Make sure to use SP Flash Tool compatible scatter file.

### Error 0xC0010004: STATUS\_UNSUPPORT\_CTRL\_CODE (0xC0010004)

**Meaning**: The SP Flash Tool version you are using doesn't support your device or chipset.

**Solution**:

1.  Make sure you are using the latest version of the SP Flash Tool.
2.  Navigate to Options > Option > Un-tick Storage Life Cycle Check.

### Error 0xC0020005: STATUS\_SEC\_IMG\_TOO\_LARGE (0xC0020005)

**Meaning**: The size of a file is larger than the available partition size, or the file isn't verified or signed.

**Solution**:

1.  Ensure that the files you're trying to flash are actually for your device's exact model.

3.  Look for different firmware/ROM.
4.  Change the phone's EMMC chip.
5.  Try using a different PC.

### Error 0xC0070005: STATUS\_DA\_EXCEED\_MAX\_NUM (0xC0070005)

**Meaning**: The SP Flas
