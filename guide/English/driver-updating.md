<img align="right" src="https://github.com/wormstest/src_vayu_windows/blob/main/2Poco X3 Pro Windows.png" width="350" alt="Windows 11 Running On A Poco X3 Pro">


# Running Windows on the POCO X3 Nfc

## Driver updating

#### Start TWRP recovery through the PC with the command

```cmd
fastboot boot <twrp.img>
```

> If you already have TWRP installed, just hold the power and vol+ buttons at startup


## Push script

```cmd
adb push msc /sbin
```

### Execute script

```cmd
adb shell sh /sbin/msc
```

## Assign letters to disks

#### Start the Windows disk manager

> Once the X3 Nfc is detected as a disk

```cmd
diskpart
```


### Assign `x` to Windows volume

#### Select the Windows volume of the phone
> Use `list volume` to find it, it's usually the one before the last

```diskpart
select volume <number>
```

#### Assign the letter x
```diskpart
assign letter=x
```

### Exit diskpart:
```diskpart
exit
```


# Install Drivers

> Replace `<suryadriversfolder>` with the location of the drivers folder

> Open cmd as administrator


```cmd
.\driverupdater.exe -d <suryariversfolder>\definitions\Desktop\ARM64\Internal\surya.txt -r <suryadriversfolder> -p X:
```


##### Boot with Windows bootable UEFI image #####

```
fastboot flash boot <uefi.img>
```

  
  

# Finished!
