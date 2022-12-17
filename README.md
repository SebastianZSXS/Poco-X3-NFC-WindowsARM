# Running Windows 11 On The Poco X3 Nfc

<img align="right" src="https://github.com/wormstest/src_vayu_windows/blob/main/Vayu-Windows11 (3).png" width="425" alt="Windows 11 Running On A Poco X3 Pro">

# ⚠️ **Warning**

We're not responsible for bricked devices, dead microSD cards, dead cats or dogs, nuclear wars or you getting fired because you forgot to boot back in to android for the alarm.

This project is in an early stage, all the files here have been contributed by other users, here you will find a guide with the working files we managed to get. This is a delicate process, do it under your own risk and follow all the steps carefully.

## Project Status

Alpha, Windows 11 boot but without USB, the next thing is to try to make the USB work

## Hardware status
### Features
- [ ] USB ```Work is underway to make it work on Windows```
- [x] UEFI buttons ```In theory is similar to Poco X3 Pro```
- [x] UFS
- [ ] Touchscreen ```Is similar to Poco X3 Pro```
- [x] Display
- [ ] Brightness
- [ ] WiFi
- [ ] Battery status
- [ ] Charging 
- [ ] GPU ```Can use driver from SC7180```
- [ ] Audio 
- [ ] Bluetooth
- [ ] Camera ```It is almost impossible in this project```
- [ ] LTE

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

- [SebastianZSXS](https://github.com/SebastianZSXS) ```Made this repo and test the progress```

- [Icesito68](https://github.com/Icesito68) ```Made windows partitioning commands and set the acpi table to the new uefi```

- [Ungeskriptet](https://github.com/ungeskriptet) ```Made uefi image of the Poco X3 NFC (Surya)```

- [Degdag](https://github.com/degdag) ```Has given me a lot of information```

- [Halal-Beef](https://github.com/halal-beef) ```Has given me a lot of information and I create the photo of the poco```
  
- [Renegade Project](https://github.com/edk2-porting) ```Making the core of this project```

- [Renegade Project Discord members](https://discord.gg/XXBWfag) ```Provided Help```
 
</details>  
