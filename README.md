# Poco-X3-NFC-WindowsARM

# Credits

- [Degdag](https://github.com/degdag) ```drivers for winpe are patched from their project for the x3 pro```

- Thanks to [ungeskriptet](https://github.com/ungeskriptet) by the uefi image of the Poco X3 NFC (Surya)

- [github edk2-msm](https://github.com/edk2-porting/edk2-msm)

- Repository based on the Special ice 68 [(Poco X3 Pro)](https://github.com/Icesito68/Port-Windows-11-Poco-X3-pro)

# Compatibility

Working: ✅|
In progess: 🔶️|
Not working: ❌


|| Aditional notes | Status |
|---------------|------------------------|--------------------------|
| USB | Powered hub needed | 🔶️|
| UFS |  | ✅|
| Display | | ✅|
| UEFI Buttons |  | ❌|
| Touchscreen | | ❌|
| WiFi | | ❌|
| Bluetooth | | ❌|
| Battery |  | ❌|
| Charge |  | ❌|
| Virtualization | it is impossible for this to work	 | ❌|
| CPU | in theory only one core should work| 🔶️|
| GPU | | ❌|
| LTE |  | ❌|
| Audio |  | ❌|
| Location |  | ❌|
| Sensors |  | ❌|
| Camera | it is almost impossible in this project	 | ❌|
| NFC | does not work on any device	 | ❌|

## Warning!
We're not responsible for bricked devices, dead microSD cards, dead cats or dogs, nuclear wars or you getting fired because the alarm app didn't work.

This is a delicate process, do it under your own risk and follow all the steps carefully.

This project is in an early stage, all the files here have been contributed by other users, here you will find a guide with the working files we managed to get.

Many information here was provided thanks to Renegade Project Discord server members.

###  Project status ### 
you will have to correct the acpi table to be able to boot windows pe

### Required Files ### 
You need to have a Recovery installed on your Poco X3 NFC [Here](https://sourceforge.net/projects/mahajant99/files/surya/TWRP/)

On PC you will need the platform-tools, you can download [Here](https://developer.android.com/studio/releases/platform-tools)

You will need a Windows compiled for ARM, choose whatever version you like [Here](https://uupdump.net/)

You need the uefi image of the Poco X3 NFC (Surya) [here](https://github.com/ungeskriptet/edk2-surya)
