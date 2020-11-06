# asus-ux305ua-hackintosh
Asus ZenBook UX305UA EFI Folder (OpenCore)

This is an EFI Folder of Asus ZenBook UX305UA Running macOS Catalina Build (19H2)

not prepped really well, but i'm pretty fine with it cause i have like 0 issues for daily use.

Detail of Specification:
- Processor : Intel Core i5-6200U
- IGPU : Intel HD Graphics 520
- RAM : 4GB 
- Storage : 1x SSD Micron m600 256GB
- Wifi : Intel AC7265 and Bluetooth
- Touchpad : ELAN0100 I2C Touchpad
- Screen Size : 13,3”
- Display Resolution : 1920 x 1080
- Bootloader : OpenCore 0.6.3
- OS : macOS Catalina 10.15.7(19H2)

List of Working hardware

- QE/CI Of Intel HD 520
- Restart, Sleep, Shutdown
- CPU Native Power Management
- Internal Speaker, Headphone jack, and internal microphone
- Brightness + Fn Keys
- Battery Indicator
- Wifi
- Bluetooth
- USB Ports 
- HDMI Out and HDMI Audio
- TouchPad
- Etc

Not Working

- Airdrop
- Headphone microphone is not detected (Port Jack issues i guess)
- Etc


Thanks to all of the developers who are providing the best work for the kext:

- thanks to https://github.com/acidanthera for providing OpenCore and other really usefull kext
- thanks to https://github.com/vit9696 for providing Lilu
- thanks to https://github.com/zxystd for providing airportitlwm & IntelBluetoothFirmware
- thanks to https://github.com/alexandred, https://github.com/coolstar, & Others for providing VoodooI2C Kext
- Others.
