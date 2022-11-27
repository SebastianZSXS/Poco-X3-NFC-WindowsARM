# Running Windows 11 On The Poco X3 Nfc

<img align="right" src="https://github.com/halal-beef/res/blob/main/vayuwindows.png" height="550">

# ⚠️ **Warning**

We're not responsible for bricked devices, dead microSD cards, dead cats or dogs, nuclear wars or you getting fired because you forgot to boot back in to android for the alarm.

This project is in an early stage, all the files here have been contributed by other users, here you will find a guide with the working files we managed to get. This is a delicate process, do it under your own risk and follow all the steps carefully.

## Project Status

Alpha 

## Hardware status
### Features
- [ ] USB ```Powered hub needed```
- [ ] UEFI buttons
- [x] UFS
- [ ] Touchscreen ```In progress!!!!```
- [x] Display
- [ ] Brightness
- [ ] WiFi
- [ ] Battery status
- [ ] Charging ```In progress```
- [ ] GPU
- [ ] Audio ```Only if it is by usb or bluetooth```
- [ ] Bluetooth
- [ ] Camera ```It is almost impossible in this project```
- [ ] LTE ```Nearly working, Windows detects it but does not allow access to the mobile network```

### Sensors
- [ ] Accelerometer
- [ ] Magnetometer
- [ ] Gyroscope 
- [ ] GPS
- [ ] Proximity
- [ ] Light sensor
- [ ] Fingerprint

## Installation instructions

<details> 

<summary><strong>All Files Needed</strong></summary>
 
- You will need the [Windows on ARM image](https://uupdump.net/) (Windows 11 is Recommended)

- [UEFI image for Poco X3 Nfc](https://github.com/SebastianZSXS/Poco-X3-NFC-WindowsARM/tree/main/UEFI)

- [TWRP](https://forum.xda-developers.com/t/recovery-3-4-0-15-surya-twrp-xiaomi-poco-x3.4167199/) for Poco X3 Nfc.

- [Magisk](https://github.com/topjohnwu/Magisk)

- On PC you will need the [Mass Storage Mode Script](https://www.mediafire.com/file/bvibrl34nawl2wg/msc.sh/file) ```This file belongs to gus33000```

- On PC you will need [platform-tools](https://developer.android.com/studio/releases/platform-tools).

- On PC you will also need a [program](https://github.com/WOA-Project/DriverUpdater/releases/) to install the [drivers](I hope soon)

- We will need [parted](https://drive.google.com/file/d/1e8kDC2fylkvJuHimlViHOuHyk8xljr6p/view) for partitioning.
  
 </details> 

### Commands

**Make sure to install TWRP, Magisk And The Magisk Module Before Proceeding.**

[Do these commands](https://github.com/SebastianZSXS/Poco-X3-NFC-WindowsARM/tree/main/Commands)

## Contributors

<details> 

<summary><b><strong>Credits</strong></b></summary>

- [SebastianZSXS](https://github.com/SebastianZSXS) ```Made this repo```

- [Icesito68](https://github.com/Icesito68) ```Made windows partitioning commands ```

- [Ungeskriptet](https://github.com/ungeskriptet) ```Made uefi image of the Poco X3 NFC (Surya)```

- [Degdag](https://github.com/degdag) ```Has given me a lot of information```

- [Halal-Beef](https://github.com/halal-beef) ```Has given me a lot of information```
  
- [Renegade Project](https://github.com/edk2-porting) ```Making the core of this project```

- [Renegade Project Discord members](https://discord.gg/XXBWfag) ```Provided Help```
 
</details>  
