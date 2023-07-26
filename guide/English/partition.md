<img align="right" src="https://github.com/wormstest/src_vayu_windows/blob/main/2Poco X3 Pro Windows.png" width="350" alt="Windows 11 Running On A Poco X3 Pro">


# Running Windows on the POCO X3 Nfc

## Installation

## Partitioning your device

## Notes:
> **Warning** if you delete any partitions via diskpart later on or now windows will send a ufs command that gets misinterpreted which erase all your ufs
- All your data will be erased! Backup now if needed.
- These commands have been tested.
- Ignore `udevadm` warnings
- Do not run the same command twice
- DO NOT REBOOT YOUR PHONE if you think you made a mistake, ask for help in the [Telegram chat](https://t.me/windows_on_pocox3_nfc)

#### Boot TWRP recovery through the PC with the command
```cmd
fastboot boot <twrp.img>
```
> If you already have TWRP installed, just hold the power and vol+ buttons at startup

#### Unmount all partitions
Go to TWRP settings and unmount all partitions

 ## Push necessary tools:
```cmd
adb push parted /sbin
```

## Start the ADB shell
```cmd
adb shell
```

## Create Partitions

### Give permissions
```cmd
chmod +x /sbin/*
```


### Start parted
```sh
parted /dev/block/sda
```


### Delete the `userdata` partition
> You can make sure that 16 is the userdata partition number by running
>  `print all`
```sh
rm 16
```

### Create partitions
> If you get any warning message telling you to ignore or cancel, just type i and enter

#### For 64Gb models:

- Create the ESP partition (stores Windows bootloader data and EFI files)
 ```sh
mkpart esp fat32 10.8GB 11GB
```

- Create the main partition where Windows will be installed to
```sh
mkpart win ntfs 11GB 45GB 
```

- Create Android's data partition
```sh
mkpart userdata ext4 45GB 59.4GB
```

#### For 128Gb models:

- Create the ESP partition (stores Windows bootloader data and EFI files)
```sh
mkpart esp fat32 10.8GB 11GB
```

- Create the main partition where Windows will be installed to
```sh
mkpart win ntfs 11GB 65GB
```

- Create Android's data partition
```sh
mkpart userdata ext4 65GB 123GB
```


### Make ESP partiton bootable so the EFI image can detect it
```sh
set 16 esp on
```

### Quit parted
```sh
quit
```

### Reboot to TWRP

### Start the shell again on your PC
```cmd
adb shell
```

### Format partitions
-  Format the ESP partiton as FAT32
```sh
mkfs.fat -F32 -s1 /dev/block/by-name/esp -n ESPSURYA
```

-  Format the Windows partition as NTFS
```sh
mkfs.ntfs -f /dev/block/by-name/win -L WINSURYA
```

- Format data
Go to Wipe menu and press Format Data, 
then type `yes`.

### Check if Android still starts
just restart the phone, and see if Android still works


## [Next step: Install Windows](https://github.com/SebastianZSXS/Poco-X3-NFC-WindowsARM/blob/main/guide/English/install.md)
