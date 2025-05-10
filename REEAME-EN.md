### Phone is totally dead

  
Message: Phone no longer responds to power button  
  
Solution:  

*   Follow this guide @ [https://www.hovatek.com/forum/thread-286.html](https://www.hovatek.com/forum/thread-286.html)  
    

  

### Phone still not working after flashing

  
Message: Phone still stuck at Bootlogo or Bootloop  
  
Solution: 

*   Ensure there's a formatted SD card in the phone before flashing  
    
*   Give up to 5 minutes because first boot takes time  
    
*   Boot the phone into recovery mode then wipe data / factory reset  
    
*   Remove the battery for 30 seconds then slot back in  
    
*   Try a firmware upgrade . use MTK droid tools version 2.3.0 to backup usrdata & cache or copy then from the clockworkmod backup  
    
*   Try a firmware / ROM from another source  
    

  

### Phone shows white screen, strange colors or divided screen after flashing

  
Message: You can see the phone responding to buttons and making sound but all is blurred by white screen  
  
Solution:  

*   The ROM / Firmware you flashed is incompatible, get from another source (especially boot.img , logo.bin and uboot.bin / lk.bin )  
    

  

### Phone automatically disconnecting during flashing

  
Message: The phone makes the disconnecting sound just as flashing begins, interrupting the process  
  
Solution: 

*   Try a different USB cord, USB port & PC  
    
*   Try holding down the Volume decrease (you could try volume increase or both) while connecting the phone to PC for flashing  
    
*   Launch Device manager (Right-click My Computer > Select Manage)  
    
*   Connect the phone to the PC via a USB cord, Device manager should refresh  
    
*   Take note of what the phone is detected as (often as Unknown or Mediatek under Other devices)  
    
*   Right-click whatever the phone is detect as and select Update Driver Software...  
    
*   Select Browse my computer for driver software  
    
*   Select Let me pick from a list of device drivers on my computer  
    
*   Click Next  
    
*   Click Have Disk  
    
*   Proceed with the Mediatek (VCOM) driver installation steps described at [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html) and click Yes if you get an Update Driver warning  
    

  

### Sp Flash tool remains at 0%

  
Message: Phone only shows charging sign  
  
Meaning: Necessary drivers have not been successfully installed on the PC  
  
Solution: 

*   Follow this guide @ [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  to manually install vcom drivers  
    
*   If you have installed VCOM drivers but the phone is still only charging then Launch Device manager (Right-click My Computer > Select Manage)  
    
*   Connect the phone to the PC via a USB cord, Device manager should refresh  
    
*   Take note of what the phone is detected as (often as Unknown or Mediatek under Other devices)  
    
*   Right-click whatever the phone is detect as and select Update Driver Software...  
    
*   Select Browse my computer for driver software  
    
*   Select Let me pick from a list of device drivers on my computer  
    
*   Click Next  
    
*   Click Have Disk  
    
*   Proceed with the Mediatek (VCOM) driver installation steps described at [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html) and click Yes if you get an Update Driver warning  
    

  

### Stuck at Download DA 100%

  
Message: Download DA 100%  
  
Meaning: SP Flash tool is having trouble communicating with the device  
  
Solution:  
Uninstall and re-install Mediatek drivers  
  

### Error 5054

  
Message: BROM ERROR S\_DL\_GET\_DRAM\_SETTINGS\_FAIL (5054)   
  
Meaning: The files you're trying to flash do not belong to or are not compatible with the phone you're trying to flash them to OR if you're getting the error while trying to format then it's likely you only loaded scatter file without the rest of the files in the firmware  
  
Solution: 

*   If you're trying to flash firmware, then ensure you're using the correct files. If you're sure they are, then try formatting before flashing again  
    
*   If you're trying to format, then ensure you the scatter file you loaded onto SP flash tool has complete firmware file locations  
    

  

### Initialize scatter failed

  
Message: Error: Initialize scatter file failed. Please check the scatter file name you load is legal  
  
Meaning: SP Flash tool doesn't accept the name format of your scatter file  
  
Solution: 

*   Ensure the scatter file wasn't renamed. If you're certain it wasn't, try a higher version of SP Flash tool  
    

  

### Error 8038

  
Message: Error 8038! Android download  pmt is ready and layout has been changed  
  
Meaning: SP Flash tool is having trouble writing to certain partitions due to some incompatibility   
  
Solution: 

*   Format the phone in SP flash tool (Do not format Bootloader) then try flashing the files again using Download  
    
*   If Download doesnt work then do a firmware upgrade  
    
*   If the MTK backup contains more than one scatter file, retry flashing with the other scatter file.  
    
*   If that isn't feasible, try formatting first or use firmware upgrade  
    
*   If that doesn't work, open the scatter file using Notepad++ and change \_\_NODL\_FAT to FAT by removing "\_\_NODL\_" .   
    

  

### Error 4032

  
Message: BROM ERROR : S\_FT\_ENABLE\_DRAM\_FAIL (4032) \[EMI\] Enable DRAM fail  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    
*   Probably have the wrong driver installed. Uninstall vcom,  preloader and MTK drivers using usb deview then manually re-install using  [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    
*   Delete the sp flash tool folder then re-extract  
    
*   Ensure the phone is switched off (with battery still inside) before connecting to PC for flashing.  
    
*   If that doesn't work, keep  holding  down the volume decrease button just before connecting the phone to PC for flashing (you could try volume increase , power + volume decrease or power + volume increase).  
    
*   Consider using the latest version of Sp Flash tool  
    
*   Format the phone before trying to flash the file(s) again  
    

  

### Error 5056

  
Message: BROM ERROR : S\_DL\_PMT\_ERR\_NO\_SPACE (5069)  
  
Meaning: The size of a file is larger than the available / possible partition size  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Try another stock ROM  
    
*   Change the phone's emmc chip  
    

  

### Error 4001

  
Message: S\_FT\_DA\_NO\_RESPONSE or Da didn't send response data to FlashTool!  
  
Meaning: SP flash tool is having difficulty communicating with the device  
  
Solution: 

*   Change the USB-port   
    
*   Run SP flash tool as Admin  
    
*   Ensure to install the correct drivers (see [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html) )  
    
*   Try another PC and USB cord  
    
*   Ensure the phone is switched off with a charged battery inside when connecting to the PC for flashing  
    

  

### Sp flash tool was successful but phone's calibration doesn't work

  
Message: Soft keys and touch screen don't work / respond  
  
Solution:

*   Edit the scatter file using Notepad++ and remove NODL\_\_  (or set is\_download: false to is\_download: true ) in front of the items you have in the backup folder but aren't listed when you load the scatter file in SP flash tool. This way, these items will become listed when  next you load the scatter file (after saving of course) and therefore flashable  
    

  

### Error 4008

  
Message: BROM ERROR : S\_FT\_DOWNLOAD\_FAIL (4008)  
  
Meaning: SP Flash tool encountered an error while attempting to flash files  
  
Solution: 

*   Ensure the battery is in the phone and the phone is switched off before connecting for flashing  
    
*   Try using a higher version of SP flash tool  
    
*   Change the USB cord and port or PC  
    
*   Use the format option then download in SP flash tool  
    

  

### Error 3149

  
Message: BROM ERROR : S\_DA\_SDMMC\_WRITE\_FAILED (3149)  
  
Meaning: SP Flash tool was unable to flash files to the phone  
  
Solution:

*   Ensure to run the latest version of SP flash tool as Administrator  
    
*   Format first then Download  
    
*   Don't tick a box with an unspecified / empty file path  
    
*   Ensure the phone is switched off (with a well charged battery in it ) before connecting to PC for flashing  
    
*   Try a different PC  
    
*   Try a different ROM  
    
*   Try a different USB cord  
    
*   Try formatting the phone first before flashing files to it  
    

  

### Error 3168 

  
Message: BROM ERROR: S\_CHIP\_TYRE\_NOT\_MATCH(3168)  
  
Meaning: Sp flash tool believes there's a mismatch between the information provided in the scatter file and the phone's info.  
  
Solution:

*   Ensure you're using the ROM for the exact phone model  
    
*   Try a higher version of SP flash tool  
    
*   Ensure to install the correct drivers for the phone on the PC  
    

  

### Error 2004 

  
Message: BROM ERROR : S\_FT\_DOWNLOAD\_FAIL (2004)  
  
Meaning: There was an interruption in the communication between SP flash tool and the device  
  
Solution:

*   A Secure Boot Download Agent (DA) might be required  
    
*   Take out and reinsert the battery  
    
*   Try using a different USB cord, port and PC  
    
*   Right-click flash\_tool.exe > Select Properties > Select Compatibility > Set to Windows XP Service Pack 3 > Click Apply > Click OK > Run SP flash tool as Administrator  
    
*   Try a different USB cord  
    
*   Try a different port on the PC or another PC  
    
*   Ensure the battery is well changed and inside the switched off phone before connecting to PC for flashing  
    

  

### USB device not recognized

  
Message: USB device not recognized prompt at system tray after connecting  the phone to PC  
  
Meaning: The PC is having problems communicating with the phone (often due to interruption, hardware or driver problems)  
  
Solution:

*   Follow the guide @ [https://www.hovatek.com/forum/thread-808.html](https://www.hovatek.com/forum/thread-808.html)  
    
*    Try a different USB cord, PC port or PC  
    

  

### Error 1013 

  
Message: BROM ERROR:S\_COM\_PORT\_OPEN Fail(1013)  
  
Meaning: SP flash tool encountered an error while attempting to communicate with the phone via the target port  
  
Solution:

*   Try using a different port on the PC  
    
*   Try a different version of SP flash tool  
    
*   Install VCOM drivers using  [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    
*   Ensure the phone is switched off with battery inside before connecting to the PC for flashing  
    
*   Try using a different PC  
    
*   Try changing the USB cord  
    
*   Ensure the phone's USB port isn't damaged  
    

  

### Error 2020 

  
Message: BROM ERROR : S\_BROM\_CHKSUM16\_MEM\_RESULT\_DIFF (2020)  
  
Meaning: SP flash tool encountered a problem moving the files to be flashed into the phone's internal SRAM  
  
Solution:

*   Use the latest version of SP flash tool  
    
*   In SP flash tool, navigate to Options > Option > Connection > Battery. Set it to "with battery".  
    
*   Use the Format all + Download option  
    
*   Hold both volume buttons before connecting to the PC for flashing and release once flashing begins  
    

  

### Error 5007 

  
Message: BROM ERROR : S\_FTHND\_FILE\_IS\_NOT\_LOADED\_YET (5007)  
  
Meaning: You're trying to flash an item with an unspecified path (no file selected for the ticked item/box)  
  
Solution:

*   Ensure the scatter file is in the same directory as the other file(s) to be flashed  
    
*   Untick any item whose file you do not have or whose path is not specified; yet, is ticked / selected for flashing  
    

  

### Error 4010

  
Message: BROM ERROR : S\_FT\_FORMAT\_FAIL  
  
Meaning: The blocks map in the scatter file doesn't match the phone's partition sizes  
  
Solution:

*    Try using the latest version of Sp flash tool  
    
*   Try using another firmware for the exact phone model  
    

  

### Error 3182

  
Message: BROM ERROR: S\_STORAGE\_NOT\_MATCH (3182)  
  
Meaning: The ROM your're trying to flash is not compatible with the target device  
  
Solution:

*   Download the ROM for the exact phone model you're trying to flash  
    
*   Ensure to install VCOM drivers on the PC  
    
*   Don't tick any box (after loading the scatter file) without a file path / whose corresponding file has not been automatically or manually loaded.  
    

  

### Error 6012

  
Message: BROM ERROR: S\_SECURITY\_SF\_CODE\_COMMAND\_FORBIDDEN (6012), MSP ERROR CODE: 0X00  
  
Meaning: The Download-Agent being used is incompatible with the phone  
  
Solution:

*   Set Download-Agent to MTK\_AllInOne\_DA.bin  
    

  

### Error 1042

  
Message: BROM ERROR: S\_TIMEOUT (1042)  
  
Meaning: The flashing process took too long so SP flash tool encountered a timeout  
  
Solution:

*   Try flashing one file at a time  
    
*   Use the latest version of SP flash tool  
    
*   Try using a different PC and USB cord  
    
*   Try Infinix Flash tool @ [https://www.hovatek.com/forum/thread-9224.html](https://www.hovatek.com/forum/thread-9224.html)  
    

  

### Error 2

  
Message: BROM ERROR: ?? (2)  
  
Meaning: SP Flash tool was unable to communicate with the phone  
  
Solution: 

*   Try using a different PC (preferably Windows 7 or lower)  
    
*   Install the correct VCOM drivers for your PC's OS and architecture (32 or 64 bit)  
    
*   Try another USB cord  
    

  

### Error 2005

  
Message: BROM ERROR: S\_BROM\_CMD\_STARTCMD\_FAIL (2005)  
  
Meaning: The device attempted to power on before SP flash tool could flash files to it  
  
Solution:

*   Ensure the battery is well charged  
    
*   Take out and reinsert the battery  
    
*   Try using a different USB cord, port and PC  
    
*   Right-click flash\_tool.exe > Select Properties > Select Compatibility > Set to Windows XP Service Pack 3 > Click Apply > Click OK > Run SP flash tool as Administrator  
    
*   Try a different USB cord  
    
*   Try a different port on the PC or another PC  
    
*   Ensure the battery is well changed and inside the switched off phone before connecting to PC for flashing  
    
*   Do not hold any button when connecting to PC  
    

  

### Error 4058

  
Message: BROM ERROR: S\_FT\_GET\_MEMORY\_FAIL (4058)  
  
Meaning: SP flash tool was unable to locate the partition you're trying to flash to  
  
Solution:

*   Untick any item (box) with a blank or empty Location  
    
*   Ensure that the memory and other components are properly seated on the board  
    

  

### Error 3178

  
Message: BROM\_ERROR\_S\_STORAGE\_NOT\_MATCH (3178)  
  
Meaning: The firmware you are trying to flash isnt compatible with your phone  
  
Solution:

*   Try flashing another firmware for your exact phone model / variant  
    

  

### Error 8406

  
Message: SP FLASH TOOL ERROR (8406)  
  
Meaning: There is some compatibility problem interrupting the flashing process  
  
Solution:

*   Try flashing another firmware for your exact model  
    
*   Update VCOM drivers for the device under Device manager  
    

  

### Error 1012

  
Message: BROM ERROR: S\_NOT\_ENOUGH\_MEMORY (1012)  
  
Meaning: The version of SP flash tool you're using doesn't support the size(s) of the file(s) in the firmware / stock ROM.  
  
Solution:

*   Use the latest version of SP flash tool  
    

  

### Error 3140

  
Message: BROM ERROR : S\_DA\_UPDATE\_BOOLOADER\_EXIST\_MAGIC\_NOT\_MATCHED  
  
Meaning: SP flash tool encountered an error flashing a selected file to a non-specified partition  
  
Solution:

*   Try using the latest version of SP flash tool  
    
*   Use the format option then download in SP flash tool  
    

  

### Error 8417

  
Message: BROM ERROR: Initialize scatter file failed. Please check the scatter file name you load is legal  
  
Meaning: The format of the scatter file is invalid  
  
Solution:

*   Open the scatter file in Notepad++, the first line must begining with:  
      
    ############################################################################################################## General Setting #  
      
    If there is anything else above this then delete it and save the scatter file  
    

  

### Error 6047

  
Message: BROM ERROR: S\_SECURITY\_SECURE\_USB\_DL\_IMAGE\_HASH\_FAIL  
  
Meaning: Hash (integrity) check of the images being flashed failed.  
  
Solution:

*   Use SP Flash Tool V5.1516.00  
    
*   Ensure to select the right Download-Agent  
    
*   Navigate to Options > Option > Download and untick DA DLL All.....  
    

  

### Error 6010

  
Message: BROM ERROR: SP FLASHTOOL ERROR 6010 CODE DOWNLOAD FORBIDDEN  
  
Meaning: The phone has a protected bootloader  
  
Solution:

*   Untick Preloader and flash the rest  
    

  

### Error: 0xFDA

  
Message: BROM ERROR: S\_FT\_GET\_MEMORY\_FAIL (0xFDA)  
  
Meaning: SP Flash tool encountered an error reading the phone's storage  
  
Solution:

*   Try using a different USB Port, Cord and PC  
    

  

### Error 0x13BE

  
Message: S\_DL\_GET\_DRAM\_SETTING\_FAIL (0x13BE)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution:

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    

  

### Error:?? (0x3)

  
Message: BROM ERROR:?? (0x3)  
  
Meaning: SP Flash tool encountered an error maintaining a connection to the device during flashing  
  
Solution

*   Reinstall the VCOM drivers  
    
*   Try a different PC and USB cord  
    
*   The scatter file needs to be modified using [https://www.hovatek.com/forum/thread-12719.html](https://www.hovatek.com/forum/thread-12719.html)  
    

  

### PRO\_INFO: Failed to get PMT info

  
Message: PRO\_INFO: Failed to get PMT info  
  
Meaning: SP flash tool is having problems reading the phone  
  
Solution

*   Try using a different PC and USB cord  
    
*   Ensure the phone is switched off (with a charged battery inside) when you connect  
    

  

### Error 0x7D4

  
Message: BROM ERROR: S\_BROM\_DOWNLOAD\_DA\_FAIL  
  
Meaning: SP Flash tool encountered an error writing to the phone  
  
Solution

*   Try changing the Download Agent (Secure Boot DA)  
    
*   Try using a different USB cord, PC port and PC  
    
*   Use the latest version of SP flash tool  
    
*   Ensure the battery is well charged and the phone's USB port isn't faulty  
    
*   Ensure the file name matches what's in the scatter file  
    

  

### Error 6124

  
Message: BROM ERROR: S\_SECURITY\_INVALID\_PROJECT (6124), MSO ERROR CODE: 0X00  
  
Meaning: Wrong flash settings or firmware  
  
Solution:

*    Ensure you set the correct Download-Agent in SP flash tool and are using a firmware for your exact model  
    
*   Go to  Options > Option > Connection > USB Speed > Full Speed  
    
*   Go to  Options > Option > Download > Untick DA DL All with Checksum  
    

  

### Error 0x8

  
Message: BROM ERROR: ?? (0x8)  
  
Meaning: The size of a file is larger than the available / possible partition size  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Try another stock ROM  
    
*   Change the phone's emmc chip  
    
*   Try using a different PC  
    

  

### Error OXFC0

  
Message: BROM ERROR S\_FT\_ENABLE\_DRAM\_FAIL (OXFC0)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    
*   Probably have the wrong driver installed. Uninstall vcom,  preloader and MTK drivers using usb deview then manually re-install using  [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    
*   Delete the sp flash tool folder then re-extract  
    
*   Ensure the phone is switched off (with battery still inside) before connecting to PC for flashing.  
    
*   If that doesn't work, keep  holding  down the volume decrease button just before connecting the phone to PC for flashing (you could try volume increase , power + volume decrease or power + volume increase).  
    
*   Consider using the latest version of Sp Flash tool  
    
*   Format the phone before trying to flash the file(s) again  
    

  

### Error 0X411

  
Message: BROM ERROR: S\_CHKSUM\_ERROR (0X411)  
  
Meaning: There was a checksum error when flashing the firmware  
  
Solution

*   Delete any file with checksum in its name from the firmware folder  
    
*   Go to Options > Option > Download > Untick Da DL all with checksum  
    

  

### Error 0xFA1

  
Message: BROM ERROR : S\_FT\_DA\_NO\_RESPONSE (0xFA1)  
  
Meaning: SP Flash tool encountered an error communicating with the device  
  
Solution

*   Try using a different port, PC and USB cord  
    
*   Ensure the phone is switched off with a charged battery inside  
    
*   Do not hold any button when connecting for flashing  
    
*   Ensure to install VCOM drivers @ [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    

  

### Error 4017

  
Message: BROM ERROR: S\_FT\_NAND\_READLEN\_NOT\_ALIGNMENT (4017)  
  
Meaning: You're trying to flash a file that has not been processed for flashing in SP flash tool  
  
Solution:

*   If you're using an MTK Droid tools backup then ensure to carry out Phase II @ [https://www.hovatek.com/forum/thread-468.html](https://www.hovatek.com/forum/thread-468.html)  
    

  

### TOOL DL image Fail !

  
Message: TOOL DL image Fail !  
  
Meaning: The firmware was flashed with Da DL all with Checksum disabled  
  
Solution:

*   In SP flash tool, navigate to Options > Option > Download > Tick Da Dl all with checksum > Reflash the firmware  
    

  

### Please select one ROM at least before execution

  
Message: Please select one ROM at least before execution  
  
Meaning: SP flash tool fails to recognize that there is an item ticked  
  
Solution:

*   Select the scatter file again and untick all items you do not wish to flash one after the other. Don't use the checkbox beside "Name" in SP flash tool  
    

  

### Error 0xFC0

  
Message: BROM ERROR : S\_FT\_ENABLE\_DRAM\_FAIL (0xFC0)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    
*   Probably have the wrong driver installed. Uninstall vcom,  preloader and MTK drivers using usb deview then manually re-install using  [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    
*   Delete the sp flash tool folder then re-extract  
    
*   Ensure the phone is switched off (with battery still inside) before connecting to PC for flashing.  
    
*   If that doesn't work, keep  holding  down the volume decrease button just before connecting the phone to PC for flashing (you could try volume increase , power + volume decrease or power + volume increase).  
    
*   Consider using the latest version of Sp Flash tool  
    
*   Format the phone before trying to flash the file(s) again  
    

  

### Error: 0xC0050003

  
Message: BROM ERROR: STATUS\_DOWNLOAD\_EXCEPTION (0xC0050003)  
  
Meaning: There was an interruption during writing to one or more partitions  
  
Solution:

*   Repeat flashing with the latest version of SP Flash Tool  
    
*   Try using a different Port, USB cord and PC  
    
*   Try flashing one partition at a time to figure out which partition results to the error  
    
*   Try flashing using a different software e.g miracle thunder, cm2 or any other dongle tool you might have  
    

  

### Error: 0xc002002A

  
Message: BROM ERROR: STATUS\_SEC\_IMG\_TYPE\_MISMATCH (0xc002002A)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device, you have selected the wrong flashing settings or verified boot is enabled  
  
Solution: 

*   Try unlocking the bootloader before flashing  
    
*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    
*   Probably have the wrong driver installed. Uninstall vcom,  preloader and MTK drivers using usb deview then manually re-install using  [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    
*   Delete the sp flash tool folder then re-extract  
    
*   Ensure the phone is switched off (with battery still inside) before connecting to PC for flashing.  
    
*   If that doesn't work, keep  holding  down the volume decrease button just before connecting the phone to PC for flashing (you could try volume increase , power + volume decrease or power + volume increase).  
    
*   Consider using the latest version of Sp Flash tool  
    
*   Format the phone before trying to flash the file(s) again  
    
*   For transsion phones (e.g tecno, infinix, itel, e.t.c ) running android 10, flash the device using latest cm2 mtk module @ [https://www.hovatek.com/forum/thread-21827.html](https://www.hovatek.com/forum/thread-21827.html)  
    

  

### Error 0XFA8

  
Message: BROM ERROR: S\_FT\_DOWNLOAD\_FAIL (0XFA8)  
  
Meaning: SP Flash tool encountered an error while attempting to flash files  
  
Solution: 

*   Ensure the battery is in the phone and the phone is switched off before connecting for flashing  
    
*   Try using the latest version of SP flash tool  
    
*   Change the USB cord and port or PC  
    
*   Use the format option then download in SP flash tool  
    
*   Try changing the Download Agent setting in SP Flash tool  
    

  

### Error 0x7D5

  
Message: BROM ERROR: S\_BROM\_CMD\_STARTCMD\_FAIL (0x7D5)  
  
Meaning: The device attempted to power on before SP flash tool could flash files to it  
  
Solution:

*   Ensure the battery is well charged  
    
*   Take out and reinsert the battery  
    
*   Try using a different USB cord, port and PC  
    
*   Right-click flash\_tool.exe > Select Properties > Select Compatibility > Set to Windows XP Service Pack 3 > Click Apply > Click OK > Run SP flash tool as Administrator  
    
*   Try a different USB cord  
    
*   Try a different port on the PC or another PC  
    
*   Ensure the battery is well changed and inside the switched off phone before connecting to PC for flashing  
    
*   Do not hold any button when connecting to PC  
    

  

### Boundary Check Failed

  
Message: Boundary Check Failed: rom\_end\_addr >= next rom begin\_addr.  
  
Meaning: The firmware has a partition that wasn't included while backing up the firmware. SP flash tool encounters an error in the end address of the preloader partition and the begin address of PGPT partition (i.e the partition which wasn't included in the backup)  
  
Solution:

*   Close the error message,  then manually select the location of all files in the scatter file from the bottom to the top. Meaning that preloader would be the last thing you'll select  
    
*   If that doesn't work, open and modify the scatter file using Notepad++ then change "boundary\_check: True" to "boundary\_check: False"  
    
*   If after modifying the scatter file and you still encounter the same or a different error, then flash the firmware using miracle box @ [https://www.hovatek.com/forum/thread-14106.html](https://www.hovatek.com/forum/thread-14106.html)  
    

  

### Error 3179

  
Message: BROM ERROR : S\_CHIP\_TYPE\_NOT\_MATCH (3179)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    
*   Probably have the wrong driver installed. Uninstall vcom,  preloader and MTK drivers using usb deview then manually re-install using  [https://www.hovatek.com/forum/thread-440.html](https://www.hovatek.com/forum/thread-440.html)  
    
*   Delete the sp flash tool folder then re-extract  
    
*   Ensure the phone is switched off (with battery still inside) before connecting to PC for flashing.  
    
*   If that doesn't work, keep  holding  down the volume decrease button just before connecting the phone to PC for flashing (you could try volume increase , power + volume decrease or power + volume increase).  
    
*   Consider using the latest version of Sp Flash tool  
    
*   Format the phone before trying to flash the file(s) again  
    

  

### Error 5073

  
Message: BROM ERROR : S\_DL\_READ\_PT\_FAIL (5073)  
  
Meaning: SP flash tool encountered an error while trying to format the device  
  
Solution: 

*   Use "download only" under the download tab to flash the firmware then you can format if need be.  
    

  

### SP Flash Tool force-closes when scatter file is loaded

  
Message: SP Flash tool automatically closes after selecting a scatter file  
  
Meaning: SP Flash Tool doesn't support the scatter file due to its blocks or configuration  
  
Solution:

*   Open the scatter file using Notepad++ >  Locate the last partition on the list (flashinfo) > change is\_download from true to false > Save the scatter file and reload  
    

  

### Storage type mismatch!

  
Message: scatter storage type is HW\_STORAGE\_EMMC  
target storage type is HW\_STORAGE\_NAND  
  
Meaning: There's a mismatch between the phone's storage type and that which the scatter file expects  
  
Solution:

*   Try using a different firmware or a Chinese box @ [https://www.hovatek.com/forum/forum-97.html](https://www.hovatek.com/forum/forum-97.html)  
    
*   Try a different version of SP Flash tool and run as Administrator  
    

  

### Error 8045

  
Message: No Valid Partition Management Table (PMT) for storage  
  
Meaning: SP Flash tool encountered a problem identifying the device's partitions ahead of file writes  
  
Solution:

*   Try Flashing the firmware using Download only  
    

  

### Error 1041

  
Message: BROM ERROR: S\_CHKSUM\_ERROR (1041)  
  
Meaning: There was a checksum error when flashing the firmware  
  
Solution

*   Delete any file with checksum in its name from the firmware folder  
    
*   Go to Options > Option > Download > Untick Da DL all with checksum  
    

  

### 0x00

  
Message: BROM ERROR: S\_SECURITY\_AC\_REGION\_NOT\_FOUND\_IN\_SECROIMG (6128), MSP ERROR CODE: 0X00  
  
Meaning: The ROM contains a Checksum file but DL All With CheckSum was unticked  
  
Solution:

*   Ensure to tick DL All With CheckSum under Options > Option > Download  
    

  

### BROM ERROR : S\_SECURITY\_SECRO\_HASH\_INCORRECT (6126) , MSP ERROE CODE : 0x00

  
Message: BROM ERROR : S\_SECURITY\_SECRO\_HASH\_INCORRECT (6126) , MSP ERROE CODE : 0x00  
  
Meaning: The ROM contains a Checksum file but DL All With CheckSum was unticked  
  
Solution:

*   Ensure to tick DL All With CheckSum under Options > Option > Download  
    

  

### Error 0xC0050005

  
Message: ERROR STATUS\_EXT\_RAM\_EXCEPTION (0xC0050005)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution:

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Ensure you tick the boxes for only the files present in the ROM you're about to flash  
    
*   Ensure that the battery of your device is well charged  
    
*   Try the technique used @ [https://www.hovatek.com/blog/my-experien...g-stylo-6/](https://www.hovatek.com/blog/my-experience-unbricking-a-dead-boot-lg-stylo-6/)  
    

  

### Error (3)

  
Message: BROM ERROR: ?? (3)  
  
Meaning: There's a problem with the format of the scatter file or file(s) being flashed. An example is trying to flash .bin files using SP Flash Tool  
  
Solution:

*   Check the scatter file and files you're about flashing to be sure they're not meant to be flashed using a different tool  
    

  

### Error 6104

  
Message: BROM ERROR: S\_SECURITY\_SECURE\_USB\_DL\_DA\_RETURN\_INVALID\_TYPE (6104), MSP ERROR CODE : 0X00  
  
Meaning: Wrong flash settings or firmware  
  
Solution:

*    Ensure you set the correct Download-Agent in SP flash tool and are using a firmware for your exact model  
    
*   Go to  Options > Option > Connection > USB Speed > Full Speed  
    
*   Go to  Options > Option > Download > Untick DA DL All with Checksum  
    

  

### Error 3183 

  
Message: BROM ERROR: S\_CHIP\_TYRE\_NOT\_MATCH(3183)  
  
Meaning: Sp flash tool believes there's a mismatch between the information provided in the scatter file and the phone's info.  
  
Solution:

*   Ensure you're using the ROM for the exact phone model  
    
*   Try a higher version of SP flash tool  
    
*   Ensure to install the correct drivers for the phone on the Pc  
    

  

### Error 0xC0060001

  
Message: BROM ERROR: S\_BROM\_CMD\_STARTCMD\_FAIL (0xC0060001)  
  
Meaning: The device attempted to power on before SP flash tool could flash files to it  
  
Solution:

*   The device might require a custom Download Agent (DA) to be flashed  
    
*   Go to Options > Option > Connection and set connection to USB high speed auto detect. Only choose UART when you have a device detected in the chosen UART port  
    
*   Ensure the battery is well charged  
    
*   Take out and reinsert the battery  
    
*   Try using a different USB cord, port and PC  
    
*   Right-click flash\_tool.exe > Select Properties > Select Compatibility > Set to Windows XP Service Pack 3 > Click Apply > Click OK > Run SP flash tool as Administrator  
    
*   Try a different USB cord  
    
*   Try a different port on the PC or another PC  
    
*   Ensure the battery is well changed and inside the switched off phone before connecting to PC for flashing  
    
*   Do not hold any button when connecting to PC  
    

  

### PMT changed for the ROM

  
Message: PMT changed for the ROM; it must be downloaded  
  
Meaning: The partition table about to be written (from the scatter file) is different from the phone's current partition table layout  
  
Solution:

*   Ensure that the scatter file / files you're trying to flash are actually for your exact model  
    
*   If you're trying to flash just a few files and not the firmware then you need to get the firmware to complement and then flash using download only  
    
*   If you're trying to flash the full firmware then try using the Firmware Upgrade option or Format first before download only  
    

  

### Error 6004

  
Message: ERROR: S\_SECURITY\_SLA\_FAIL (6004), MSP ERROE CODE: 0X00  
  
Meaning: The download agent isn't compatible with the device  
  
Solution:

*   Try choosing a different Download Agent, version or tool  
    
*   Ensure you're using the right Authentication file  
    

  

### Storage type mismatch!

  
Message:  
scatter storage type is HW\_STORAGE\_EMMC  
target storage type is HW\_STORAGE\_NONE  
  
Meaning: There's a mismatch between the phone's storage type and that which the scatter file expects  
  
Solution:

*   Try using SP Flash tool Version 3.x  
    

  

### Error 6045

  
Message: S\_SECURITY\_SECURE\_USB\_DL\_IMAGE\_SIGN\_HEADER\_NOT\_FOUND (6045) , MSP ERROE CODE : 0x00  
  
Meaning: The image files you are trying to flash doesn't contain the -sign header.  
  
Solution:

*   Use SP Flash Tool V5.1532.00 @ [https://www.hovatek.com/forum/thread-13970.html](https://www.hovatek.com/forum/thread-13970.html)  
    
*   Load the Auth file for the device in the flash tool  
    
*   Ty flashing a factory (signed) firmware  
    
*   Flash the unsigned image using the 'Write Memory' tab in SP flash tool. To activate write memory tab, press 'Ctrl + Alt + V' to enabled advanced mode then click Window > Write Memory  
    

  

### Error 2035

  
Message: BROM ERROR: S\_BROM\_CMD\_JUMP\_DA\_FAIL (2035)  
  
Meaning: SP Flash tool encountered an error connecting to the device.  
  
Solution

*   Ensure the battery is inserted and you're not holding any button when connecting to PC for flashing  
    
*   Uninstall all Mediatek drivers then re-install VCOM drivers  
    
*   Disable any modem manager or software which might be blocking ports on the PC  
    
*   For Linux / Ubuntu users, make sure you installed libusb-dev then blacklist Ubuntu’s modem manager (because it controls port /dev/ttyACM0, which is disabling SP Flash Tool from running properly).  
    

  

### Error 0x412

  
Message: BROM ERROR: S\_TIMEOUT (0X412)  
  
Meaning SP Flash tool encountered a timeout when trying to flash (i.e flashing took too long to start or complete)  
  
Solution

*   Ensure that files are actually loaded (with valid location) in SP flash tool (i.e location should not be empty)  
    
*   Try flashing one file at a time  
    
*   Use a higher version of SP Flash tool  
    
*   Untick the large files or find smaller alternatives  
    

  

### Error 6029

  
Message: S\_SECURITY\_SEND\_AUTH\_FAIL (6029) , MSP ERROE CODE : 0x00  
  
Meaning SP Flash tool can't authenticate the files you are trying to flash  
  
Solution

*   Try another ROM / firmware from a different source  
    
*   Get an Auth file for your phone model  
    
*   For Tecno, Infinix & Itel devices, use Software Download tool (Format + Download)  
    

  

### Error 0x93AF

  
Message: ROM\[logo\] checksum mismatch checksum\_config\[0x93af\],checksum\_val\[0x94ae\]  
  
Meaning SP Flash tool encountered a checksum error  
  
Solution

*   Open the checksum file using notepad++, search for 0x93af and replace with 0x94ae  
    
*   Delete any checksum file in the rom  
    

  

### Error 5011

  
Message: S\_DL\_SCAT\_INCORRECT\_FORMAT (5011)  
  
Meaning The scatter file has incorrect format. The scatter file has been badly created / modified  
  
Solution

*   Download a different scatter file (one that doesn't pop the same incorrect scatter file error in SPft), open the two scatter files using Notepad++ and you will notice that the incorrect scatter file has its items slightly shifted to the left. Edit the incorrect scatter file to the same format arrangement as in the working scatter file.  
    
*   After modifying the scatter file using the method above, ensure to use a recent version of SP flash tool e.g SP flash tool v5.1728  
    
*   Download another ROM / firmware from a different source  
    

  

### Error 0xC52

  
Message: ERROR: S\_DA\_SDMMC\_WRITE\_FAILED (0XC52)  
  
Meaning: SP Flash tool was unable to flash files to the phone  
  
Solution:

*   Ensure to run the latest version of SP flash tool as Administrator  
    
*   Format first then Download  
    
*   Don't tick a box with an unspecified / empty file path  
    
*   Ensure the phone is switched off (with a well charged battery in it ) before connecting to PC for flashing  
    
*   Try a different PC  
    
*   Try a different ROM  
    
*   Try a different USB cord  
    
*   Try formatting the phone first before flashing files to it  
    

  

### Error 0XFAA

  
Message: BROM ERROR: S\_FT\_FORMAT\_FAIL (0XFAA)  
  
Meaning: The source (firmware) doesn't properly match the target (phone)  
  
Solution:

*   Try using a different firmware for your phone model  
    
*   Ensure you're using the right tool to flash the firmware  
    

  

### Error 5072

  
Message: ERROR: S\_DL\_WRITE\_PT\_FAIL (5072)  
  
Meaning: SP flash tool is having problems writing to one or more partitions  
  
Solution

*   Try using a different PC and USB cord  
    
*   Ensure the phone is switched off (with a charged battery inside) when you connect  
    
*   Do not hold any button when connecting to PC for flashing  
    

  

### Error 0xC0070004

  
Message: ERROR: STATUS\_DA\_HASH\_MISMATCH (0xC0070004)  
  
Meaning: Hash (integrity) check of the images being flashed failed.  
  
Solution:

*   Use SP Flash Tool V5.1516.00  
    
*   Ensure to select the right Download-Agent  
    
*   Navigate to Options > Option > Download and untick DA DLL All.....  
    
*   Try a different firmware build  
    

  

### Error 6046

  
Message: BROM ERROR: S\_SECURITY\_USB\_DL\_IMAGE\_SIGNATURE\_VERIFY\_FAIL (6064), MSP ERROR CODE: 0X0  
  
Meaning: Signature verification for the firmware failed  
  
Solution:

*   Set Download-Agent to MTK\_AllInOne\_DA.bin  
    
*   Navigate to Options > Option > Download and untick DA DLL All.....  
    
*   Delete any checksum file in the firmware folder  
    

  

### Error 0XC0060003

  
Message: ERROR: STATUS\_BROM\_CMD\_SEND\_DA\_FAIL (0XC0060003)  
  
Meaning: SP flash tool is unable to read or write to the device using the preset Download Agent  
  
Solution:

*   The device might require a custom Download Agent (DA) to be flashed  
    
*   Ensure the battery is well charged  
    
*   Take out and reinsert the battery  
    
*   Try using a different USB cord, port and PC  
    
*   Right-click flash\_tool.exe > Select Properties > Select Compatibility > Set to Windows XP Service Pack 3 > Click Apply > Click OK > Run SP flash tool as Administrator  
    
*   Try a different USB cord  
    
*   Try a different port on the PC or another PC  
    
*   Ensure the battery is well changed and inside the switched off phone before connecting to PC for flashing  
    
*   Do not hold any button when connecting to PC  
    

  

### Error 0x94010000

  
Message: CHIP TYPE NOT match ! target refuse value: 0x94010000  
  
Meaning: The device likely has a locked / encrypted preloader  
  
Solution:

*   Untick preloader when flashing in Sp flash tool  
    

  

### Error 0xC0020029

  
Message: BROM ERROR: STATUS\_SEC\_IMGHDR\_TYPE\_MISMATCH (0xC0020029)  
  
Meaning: You are trying to flash modified files to a device that only accepts signed or verified images  
  
Solution:

*   Download and flash the official firmware (usually have -verified or -signed prefixes)  
    
*   If possible, unlock the bootloader then retry flashing  
    
*   Download the latest version of SP flash tool  
    

  

### Error 5000

  
Message: BROM ERROR : S\_AUTH\_HANDLE\_IS\_NOT\_READY (5000)  
  
Meaning: The device has a secure boot / bootloader  
  
Solution:

*   You'll need an Auth (\*.auth) or custom Download Agent (DA) file for the device to proceed with SP flash tool  
    
*   For Tecno, Infinix & Itel devices, use Software Download tool (Format + Download)  
    

  

### Error 0xC002002C

  
Message: ERROR : STATUS\_SEC\_IMG\_HASH\_VFY\_FAIL (0xC002002C)  
  
Meaning: The device has a verified boot  
  
Solution:

*   You'll need to download and flash the official firmware (usually have -verified or -sign in their file name)  
    

  

### Error 0xC0030012

  
Message: ERROR: STATUS\_SEC\_AUTH\_FILE\_NEEDED (0xC0030012)  
  
Meaning: The device has a secure boot  
  
Solution:  
You'll need to use a custom authentication file (auth) for the model  
  

### Error 0xC0060005

  
Message: ERROR: STATUS\_BROM\_CMD\_FAIL (0xC0060005)  
  
Meaning: The device attempted to power on before SP flash tool could flash files to it  
  
Solution:  
You'll need to use a custom Download Agent (DA) for the model  
  

### Error 8

  
Message: ERROR: ?? (8)  
  
Meaning: The size of a file is larger than the available / possible partition size  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Try another stock ROM  
    
*   Change the phone's emmc chip  
    
*   Try using a different PC  
    

  

### Error 5002

  
Message: ERROR: S\_INVALID\_DA\_FILE (5002)  
  
Meaning: SP flash tool does not recognize the DA file. Most likely the DA file is locked / encrypted for use on a specific tool  
  
Solution:   
You'll either need to search for a DA file compatible with SP flash tool or use the specified tool for the DA file you downloaded \[specified tool are usually hardware box / dongles e.g CM2mtk, volcano tool,  e.t.c\]  
  

### Error 0xC0030001

  
Message: Error: STATUS\_SCATTER\_FILE\_INVALID (0xC0030001)  
  
Meaning: SP flash tool does not recognize the scatter file or the location of the scatter file.  
  
Solution: 

*   Rename the folder location of the scatter file including the parent folders too, remove all special characters / non English characters from the folder name  
    
*   If that doesn't work then create a new folder in your desktop then copy and paste ONLY the firmware files into the new folder then retry flashing the contents on the new folder  
    

  

### Partition\[nvram\] should NOT set "is\_download" to true in scatter file

  
Message: Partition\[nvram\] should NOT set "is\_download" to true in scatter file  
  
Meaning: The scatter file loaded has nvram set to download but doesn't specify a file name for nvram. This error is common in later versions of SP flash tool  
  
Solution: 

*   Modify the scatter file using notepad++ and add a file name for nvram partition. e.g "file\_name: nvram.bin" then save and ensure there's an nvram.bin file in the same folder as the scatter file. If that doesn't work then  
    
*   Modify the scatter file using notepad++ and set "is\_download: false" for nvram partition  
    

  

### Error 0xC0050001

  
Message: ERROR: STATUS\_DEVICE\_CTRL\_EXCEPTION (0XC0050001)  
  
Meaning: The firmware you're trying to flash is either not compatible with your device or you have selected the wrong flashing settings  
  
Solution:

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Uninstall and re-install Mediatek drivers  
    

  

### Error 0xC002001B

  
Message: ERROR: STATUS\_SEC\_PUBK\_AUTH\_MISMATCH\_N (0xC002001B)  
  
Meaning: The device has a verified boot  
  
Solution:

*   You'll need to download and flash the official firmware (usually have -verified or -sign in their file name)  
    

  

### Error 5014

  
Message: ERROR: S\_DL\_SCAT\_ADDR\_IS\_NOT\_ASCENDING\_ORDER (5014)  
  
Meaning: The scatter file was badly created or modified, depending on how you obtained the scatter file  
  
Solution:  
Input the correct values for all 'physical\_start\_addr' in the scatter file. The correct value for 'physical\_start\_addr' is the same as the value on 'linear\_start\_addr'  
  

### Error 0x7F3

  
Message: BROM ERROR: S\_BROM\_CMD\_JUMP\_DA\_FAIL  
  
Meaning: SP Flash tool encountered an error connecting to the device.  
  
Solution

*   Ensure the battery is inserted and you're not holding any button when connecting to PC for flashing  
    
*   Uninstall all Mediatek drivers then re-install VCOM drivers  
    
*   Disable any modem manager or software which might be blocking ports on the PC  
    
*   For Linux / Ubuntu users, make sure you installed libusb-dev then blacklist Ubuntu’s modem manager (because it controls port /dev/ttyACM0, which is disabling SP Flash Tool from running properly).  
    

  

### Error 3154

  
Message: BROM ERROR : S\_DA\_SDMMC\_WRITE\_FAILED (3154)  
  
Meaning: SP Flash tool was unable to flash files to the phone  
  
Solution:

*   Ensure to run the latest version of SP flash tool as Administrator  
    
*   Format first then Download  
    
*   Don't tick a box with an unspecified / empty file path  
    
*   Ensure the phone is switched off (with a well charged battery in it ) before connecting to PC for flashing  
    
*   Try a different PC  
    
*   Try a different ROM  
    
*   Try a different USB cord  
    
*   Try formatting the phone first before flashing files to it  
    

  

### Error 0xC0010005

  
Message: BROM ERROR: STATUS\_PROTOCOL\_ERR (0xC0010005)  
  
Meaning: Sp flash tool is having problems communicating with the device  
  
Solution: Ensure the phone is properly switched off (with battery connected) before connecting to PC for flashing.  
  

### Error 0xC0010007

  
Message: BROM ERROR: INSUFFICIENT\_BUFFER (0xC0010007)  
  
Meaning: SP flash tool seems to be blocked from flashing files to the phone  
  
Solution:

*   If you can boot to fastboot mode, then unlock the bootloader then retry flashing  
    
*   Untick OEM then retry flashing  
    

  

### Error 0xC0050007

  
Message: ERROR: STATUS\_READ\_DATA\_EXCEPTION (0xC0050007)  
  
Meaning: SP flash tool is unable to readback from the connected phone (esp where the readback length is too large)  
  
Solution:

*   Download and install updated MTK drivers on your PC at \[ Login to download\]  
    
*   If you're performing a readback, try skipping cache and userdata; see [https://www.hovatek.com/forum/thread-22701.html](https://www.hovatek.com/forum/thread-22701.html)  
    

  

### Error 0x13CD

  
Message: BROM ERROR : S\_DL\_PMT\_ERR\_NO\_SPACE (5069)  
  
Meaning: The size of a file is larger than the available / possible partition size  
  
Solution: 

*   Ensure that the file(s) you're trying to flash are actually for your exact phone model  
    
*   Try another stock ROM  
    
*   Change the phone's emmc chip  
    

  

### LIB DA not match

  
Message: LIB DA not match, please re-select DA or ask for help  
  
Meaning: SP flash tool is having trouble using the selected DA file  
  
Solution: 

*   Untick 'Check LIB DA match' within SP flash tool general settings (Options > option)  
    
*   Try another version of SP flash tool @ [https://www.hovatek.com/forum/thread-13970.html](https://www.hovatek.com/forum/thread-13970.html) ; you could try v5.1828 (it doesn't have this settings)  
    

  

### Error -1073283068

  
Message: BROM ERROR: STATUS\_DA\_HASH\_MISMATCH (-1073283068), MSP ERROE CODE: 0X00  
  
  
Meaning: The DA file being used isn't compatible  
  
Solution: Try using a DA + Auth + Factory rom  
  

### Error 0XC50

  
Message: S\_DA\_SDMMC\_CONFIG\_FAILED (0XC50)  
  
Meaning: The device likely has a protected preloader or bootloader  
  
Solution: Untick preloader when flashing in Sp flash tool  
  

### Error 3152

  
Message: S\_DA\_SDMMC\_CONFIG\_FAILED (3152)  
  
Meaning: The device likely has a protected preloader or bootloader  
  
Solution: Untick preloader when flashing in Sp flash tool  
  

### Error 0xC0020006

  
Message: ERROR: STATUS\_SEC\_PL\_VFY\_FAIL (0xC0020006)  
  
Meaning: The device likely has a protected preloader or bootloader / requires on loaded for all operations  
  
Solution:

*   Ensure a preloder for your device's model is loaded before any operation  
    
*   Ensure to use the Secure Boot DA (and Auth if requested) for the device  
    
*   One or more partitions might be preventing flash. Try flashing one partition at a time  
    
*   Try using a signed firmware  
    
*   Try unlocking the bootloader before flashing  
    

  

### Error 0xC0030003

  
Message: ERROR : STATUS\_DA\_SELECTION\_ERR (0xC0030003)  
  
Meaning: The DA file being used is incompatible  
  
Solution:  
For Tecno, Infinix and Itel, try using Software Download tool @ [https://www.hovatek.com/forum/thread-23709.html](https://www.hovatek.com/forum/thread-23709.html) instead  
  

### Error 0xC0030008

  
Message: ERROR: STATUS\_INVALID\_GPT (0xC0030008)  
  
Meaning: Faulty Emmc chip on the device  
  
Solution:

*   Try writing firmware directly to emmc using an emmc tool such as UFI box  
    
*   Change the phone's emmc chip  
    

  

### Error 0xC0050004

  
Message: ERROR: STATUS\_UPLOAD\_EXCEPTION (0xC0050004)  
  
Meaning: SP Flash tool is unable to connect with the phone  
  
Solution:

*   Try a different USB cord  
    
*   Try flashing with / without battery inserted  
    

  

### Error 0x1

  
Message: ERROR: ?? (0x1)  
  
Meaning: SP Flash tool is unable to properly communicate with the phone  
  
Solution:  
Try using a custom DA & Auth file for your device model  
  

### Error 0xC0030004

  
Message: ERROR: STATUS\_PRELOADER\_INVALID 0xC0030004  
  
Meaning: There's a problem with the preloader partition name in the scatter file or communication with the device  
  
Solution:

*   Try loading the preloader from the firmware for your model before attempting to perform any operation  
    
*   Edit the scatter file preferably using Notepad++ or any other good text editor, then change partition name to all lower case e.g PRELOADER to preloader or to match the exact file name in the firmware then save the scatter file  
    
*   Try holding Vol UP or Down button before connecting the phone to the PC  
    
*   If you get the error while trying to format, return to the download tab and tick the checkbox for preloader then return to the format tab and retry formatting  
    
*   If you get the error while trying to readback, then press control + alt + v to enable advanced mode in SP flash tool, then on the readback tab, tick the checkbox for SRAM then retry the readback operation  
    
*   If readback still fails using the method above then ensure that there's a valid preloader file location within the download tab then return back to the readback tab and proceed with readback  
    

  

### Error 1003

  
Message: ERROR: S\_INVALID\_BBCHIP\_TYPE (1003)  
  
Meaning: There's a problem with the scatter file  
  
Solution:  
Ensure you're using an SP Flash tool-compatible scatter file  
  

### Error 0xC0010004

  
Message: STATUS\_UNSUPPORT\_CTRL\_CODE (0xC0010004)  
  
Meaning: The version of SP Flash tool you're using doesn't support your chipset / device or Storage Life Cycle Check is failing  
  
Solution:  
Ensure you're using the latest version of SP Flash tool then navigate to Options > Option.. > Untick Storage Life Cycle Check  
  

### Error 0xC0020005

  
Message: STATUS\_SEC\_IMG\_TOO\_LARGE (0xC0020005)  
  
Meaning: The particular file as indicated on SP flash tool is either too large in size compared to the partition on the phone or the file isn't verified or signed  
  
Solution:  
Look for and try a different firmware or search online if you'll find a replacement file (one with smaller file size) for the said partition  
  

### Error 0xC0070005

  
Message: STATUS\_DA\_EXCEED\_MAX\_NUM (0xC0070005)  
  
Meaning: The SP flash tool is having trouble communicating with the phone or you're flashing a wrong firmware  
  
Solution:

*   If you where holding vol button before connecting, then retry flashing without holding any buttons (vice versa)  
    
*   Try flashing a different firmware or at least preloader from a different firmware  
    
*   Try making a jumper connection between kcolo and gnd (something similar to [https://www.hovatek.com/forum/thread-11802.html](https://www.hovatek.com/forum/thread-11802.html) ) then flash only preloader, if successful then disconnect the jumper and flash the rest of the firmware  
    

  

### Error 0xC004000B

  
Message: ERROR: STATUS\_EXCEED\_AVALIABLE\_RANGE (0xC004000B)  
  
Meaning: You might be trying to flash or backup too many / too large partitions at a time  
  
Solution:

*   Try flashing or backing up one file / partition at a time  
    
*   Ensure you've supplied the correct partition addresses (either in scatter file or manually during readback/flash)  
    

  

### Error 0xC0010001)

  
Message: ERROR: STATUS\_ERR  (0xC0010001)  
  
Meaning DA or Auth verification failed  
  
Solution: Ensure to load a custom DA or Auth for the device or [bypass DA / Auth check](https://www.hovatek.com/forum/thread-37957.html)  
  

### Error 0xC0020004

  
Message: ERROR: STATUS\_SEC\_DL\_FORBIDDEN (0xC0020004)  
  
Meaning You aren't allowed to flash to the partition in question  
  
Solution

*   Your model might require a compatible preloader.bin always loaded for backup / flash operations  
    
*   Ensure the file you're trying to flash is factory signed / official  
    
*   Try both Write memory and Download tabs in SP flash tool  
    

  
  

### Error 0xC002004B

  
Message: ERROR: STATUS\_SEC\_INSUFFICIENT\_BUFFER (0xC002004B)  
  
Meaning The partition in question requires a -verified image  
  
Solution

*   Ensure you're using the latest version of SP flash tool  
    
*   Skip this partition when flashing (if it isn't a core partition)  
    
*   Try doing format all + download then flashing to the partition using download only (Warning: Only format a secure boot device when you either have the auth or are using the [auth bypass (SLA/DAA) tweak](https://www.hovatek.com/forum/thread-37957.html)  
    
*   Use the -verified image of that partition if the firmware contains it  
    
*   Use this [bypass method](https://www.hovatek.com/forum/thread-39260.html)  
    

  

### Error 0xC002002D

  
Message: ERROR: STATUS\_SEC\_VIOLATE\_ANTI\_ROLLBACK (0\*C002002D)  
  
Meaning The older firmware (downgrade) you're trying to flash is rejected by anti-rollback  
  
Solution  
Ensure to download firmware equal to or higher than your current build  
  

### Error 0x7009

  
Message: ERROR: brom\_scmd\_send\_auth error code 0x7009  
  
Meaning The device's chipset requires authentication to flash  
  
Solution  
Use a tool that supports server or remote authentication for the device's chipset
