# Asus ZenBook UX305UA OSX
Asus ZenBook UX305UA EFI Folder (OpenCore)

This is an EFI Folder of Asus ZenBook UX305UA Running macOS Catalina Build (19H2)

not prepped really well, but i'm pretty fine with it cause i have like 0 issues for daily use.

## Detail of Specification:
|-|-|
|-|-|
|Processor|Intel Core i5-6200U|
|IGPU|Intel HD Graphics 520|
|RAM|4GB| 
|Storage|1x SSD Micron m600 256GB|
|Wifi & Bluetooth|Intel AC7265 and Bluetooth|
|Touchpad|ELAN0100 I2C Touchpad|
|Screen Size|13,3”|
|Display Resolution|1920 x 1080(FHD)|
|Bootloader|OpenCore 0.6.3|
|OS Version|macOS Catalina 10.15.7(19H2)|
|Installer|Vanilla (macApps Store)|

---

## Functional Status

|Function / Hardware|Status|
|-|-|
|iGPU HD520 Acceleration|Working|
|CPU Power Management|Working - idles at 800MHz, boosts to max Turbo frequency|
|Laptop Keyboard|Working|
|Laptop Trackpad|Working|
|Laptop Headphones Jack|Working|
|Built-in Speakers|Working|
|Built-in Mic|Working|
|Hotkeys for audio|Working|
|USB 3.x|Working|
|Screen brightness|Working, hotkeys fn+f5/fn+f6 to decrease/increase brightness|
|Built-in Wifi|Working|
|Built-in Bluetooth|Working|
|Built-in webcam|Working|
|Sleep|Working|

---

## Bios Settings

Disabled

- VT-d
- Secure Boot
- FastBoot
- CFG-Lock (via ModGRUBShell)

Changed
- DVMT to 128Mb

---

## Disabling CFG_Lock

Make sure the modGRUBShell are in the EFI folder EFI/Tools and also have already added in config.plist>tools 

Important!
and also there might be a different value data for your CFG_Lock bios. make sure you have already following dortania post install guides (https://dortania.github.io/OpenCore-Install-Guide/)

```
setup_var_3 0x6B 0x00
reboot
```


Thanks to all of the developers who are providing the best work for the kext:

- thanks to https://github.com/acidanthera for providing OpenCore and other really usefull kext
- thanks to https://github.com/vit9696 for providing Lilu
- thanks to https://github.com/zxystd for providing airportitlwm & IntelBluetoothFirmware
- thanks to https://github.com/alexandred, https://github.com/coolstar, & Others for providing VoodooI2C Kext
- Others.
