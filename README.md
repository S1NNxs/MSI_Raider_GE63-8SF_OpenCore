## Use at your own risk!

## MSI Raider GE63-8SF OpenCore Configurations

### Laptop Specifications:
- Intel i7 8750H Cofee Lake
- Intel® HM370
- Intel UHD Graphics 630
- nVidia RTX 2070 (Disabled, HDMI disabled too)
- LAN Killer E2500 
- WLAN Intel AX200 - Replaced by Intel AX200, The original card was not tested

-------------------------------------------------------------------------------------------------
### Based on [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)

### EFI Drivers
- HFSPlus.efi
- OpenCanopy.efi
- OpenRuntime.efi

### Kexts
- [Lilu.kext](https://github.com/acidanthera/Lilu)
- [WhateverGreen.kext](https://github.com/acidanthera/WhateverGreen)
- [AppleALC.kext](https://github.com/acidanthera/AppleALC)
- [VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC)
  - [SMCProcessor.kext]
- [AtherosE2200Ethernet.kext](https://github.com/Mieze/AtherosE2200Ethernet)
- [AirportItlwm.kext](https://github.com/OpenIntelWireless/itlwm)
- [IntelBluetoothFirmware.kext](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)
  - [IntelBluetoothInjector.kext]
- [USBMap.kext](https://github.com/corpnewt/USBMap)
- [VoodooPS2Controller.kext]

### ACPI
#### :warning: AML files are configured specifically for GE63-8SF. 
#### Compatibility with other systems has not been tested. 
#### Do not use on processors other than Coffee Lake laptop!
- SSDT-AWAC-DISABLE.aml
- SSDT-EC-USBX.aml
- SSDT-KEYS.aml 
- SSDT-NoHybGfx.aml
- SSDT-PLUG.aml
- SSDT-PMC.aml
- SSDT-PNLFCFL.aml

### Config.plist
- Use [PropperTree](https://github.com/corpnewt/ProperTree) for editing .plist file (Requires Python installed on your system)
- Use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) for generating data to your config.plist (Requires for iMessage service fix)
    - [manual](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios)

### Not Working
- Battery
- Touchpad
- Sleep
- Card Reader

