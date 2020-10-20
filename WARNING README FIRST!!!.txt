REMINDERS

1 Add your SMBIOS data in config (PlatformInfo -> Generic -> Serial, UID, Motherboard)
2 If you haven't DW1560 M2 Wifi+BT Card disable and remove AirportBrcmFixup.kext, BrcmBluetoothInjector.kext, BrcmFirmwareData.kext, BrcmPatchRAM3.kext and add Intel BT drivers. (Config.plist -> Kernel -> Add)
3 Add your Mac address in config for enable Iservice etc. (PlatformInfo -> Generic -> Rom) 
take a look https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html