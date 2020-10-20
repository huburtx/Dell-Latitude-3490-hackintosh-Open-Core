# Dell-Latitude-3490-hackintosh-Open-Core-0.6.2
![banner1](https://github.com/huburtx/Dell-Latitude-3490-hackintosh-Open-Core-0.6.2/blob/master/GHContents/banner1.jpg)
</br>
![Banner](https://github.com/huburtx/Dell-Latitude-3490-hackintosh-Open-Core-0.6.2/blob/master/GHContents/banner2.jpg)


##  
| Component | Details                                                                                                         |
|:--------------:|:------------------------------------------------------------------------------------------------------------------:|
|Model |  Dell Latitude 3490 **2018**|
| CPU |    Intel Core i5 8250U (Kaby Lake) |
| GPU | Intel UHD620 |
|RAM  |    (2x8) 16GB DDR4 **(8 added)**|
| Wireless / BT  | Broadcom DW1560 (BCM94352Z) **(replaced)**<br>|
| Touchpad/Touchscreen|  DELL0839 l2C HID  |
| Sound card |  ALC256 |
|SSD | Sabrent M2 NVMe 256GB **(replaced)**<br>|
| LCD | FHD 1920*1080|
|SMBIOS | MacBookPro15,2|
| BIOS | 1.10.0 |
--------
### ⚠️I DON‘T have this laptop. 
### ⚠️The repo is created out of interest.
### ⚠️PR, Fork, issue are welcomed if you can find them.


## What's working
- [x] Intel UHD 620 with graphic accelleration
- [x] HDMI output
   - The HDMI port of `Dell Latitude 3490` is HDMI 1.4, only support 4K at 30Hz or 2k at 60Hz. If you need 4k at 60hz is reccomended Type C to DP adapter (⚠️NOT TESTED).
- [x] VGA output
- [x] Brightness Control
- [x] Backlight shortcuts (fn+F11 down, fn+F12 up)
- [x] Volume shortcuts (fn+F2 down, fn+F3 up)
- [x] USB 3.1, Type C 3.1, USB 2.0
- [x] Internal speaker
- [x] Headphone output
- [x] Internal Mic
- [x] Trackpad (All gestures, 3 and 4 fingers)
- [x] Wifi + Bluetooth (Airdrop and Iservices)
- [x] Hibernation
- [x] NVRAM
- [x] Internal camera
- [x] Ethernet
</br>


## What's not working 
-  Fingerprint sensor
-  SD card reader
</br>

## Working with issues
- Line in (Mic in) of headphone jack 
   - The `internal mic` and `line in` share the same node. In Windows, the switch is done by the driver. Need further research. If you want some layout-id can disable the internal mic.

</br>


## Post installation
   1. Install `ComboJack` to improve the headphone sound quality and enable audio from jack. 
      - [Click HERE](https://github.com/Heporis/ComboJack) to download. Credit to [Heporis](https://github.com/Heporis).
      - Execute the script in the directory below
         
         > ComboJack_Installer/install.sh
   
   **ONLY IF YOU HAVEN'T DW1560**

   2. **Realtek USB NIC Driver by [chris111](https://github.com/chris1111)**：[Link](https://github.com/chris1111/Wireless-USB-Adapter/files/4301778/Wireless.USB.Adapter-V11.zip)  
      - You may need a Realtek USB Wireless card if you haven't DW1560.

   3. **Intel Bluetooth M2 Driver by [zxystd](https://github.com/zxystd)**: [Link](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)
      - You may need Intel Bluetooth Driver if you haven't DW1560.


</br>

## Download 
   Download from Release：

   - [![Release](https://img.shields.io/github/release/huburtx/Dell-Latitude-3490-hackintosh-Open-Core-0.6.2.svg)](https://github.com/huburtx/Dell-Latitude-3490-hackintosh-Open-Core-0.6.2/releases)
</br></br>



____________
 ## Credits
 - [Acidanthera](https://github.com/acidanthera) for OpenCore (and related documents) , Lilu, AppleALC and other awesome projects.
   - [AppleALC](https://github.com/acidanthera/AppleALC)
   - [AirportBrcmFixup](https://github.com/acidanthera/airportbrcmfixup)
   - [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)
   - [CPUFriend](https://github.com/acidanthera/CPUFriend)
   - [Lilu](https://github.com/acidanthera/Lilu)
   - [OpenCore](https://github.com/acidanthera/OpenCorePkg)
   - [VoodooPS2](https://github.com/acidanthera/VoodooPS2)
   - [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
   - [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
   
- [Alex James](https://github.com/al3xtjames) for
   - [NoTouchID](https://github.com/al3xtjames/NoTouchID)

- [chris111](https://github.com/chris1111) for maintaing supports on Realtek USB wireless card.  

- [Heporis](https://github.com/Heporis) for Combojack, super ALC fix on ALC255/256.
   - [ComboJack](https://github.com/randomprofilename/ComboJack)

- [RehabMan](https://github.com/RehabMan)
   - [OS-X-Fake-PCI-ID](https://github.com/RehabMan/OS-X-Fake-PCI-ID)
   - [UsbInjectAll](https://github.com/RehabMan/OS-X-USB-Inject-All)

- [VoodooI2C Developer Team](https://github.com/VoodooI2C) for their magnificent work on I2C trackpads.  
   - [VoodooI2C](https://github.com/VoodooI2C/VoodooI2C)

- [zxystd](https://github.com/zxystd)  for awesome works on Intel wireless cards.  
   - [IntelBluetoothFirmware](https://github.com/zxystd/IntelBluetoothFirmware)

- [Mieze](https://github.com/Mieze) for Realtek Gigabit Ethernet Driver
   - [RTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/releases)
