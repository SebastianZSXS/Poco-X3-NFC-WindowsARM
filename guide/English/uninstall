<img align="right" src="https://github.com/wormstest/src_vayu_windows/blob/main/2Poco X3 Pro Windows.png" width="350" alt="Windows 11 running on a Poco X3 Pro" >

# Windows on the POCO X3 Nfc

## Restore stock partition table

### Why do we need it?

If you want to uninstall Windows use this to avoid human error to avoid writing a guide dedicated only to uninstall.

If you want to lock your bootloader again you need the stock partition table

###Previous requirements

- [gpt_both0.bin](../../../../releases/label/Binaries)

### Grades

> Replace ```<gpt_both0.bin>``` with the directory of gpt_both0.bin


## GPT Restaurant

``` cmd
fastboot flash partition: 0 <gpt_both0.bin>
```

## Format user data to avoid bootloop and restore FS weight
``` cmd
fastboot -w
```
