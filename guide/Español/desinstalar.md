<img align="right" src="https://github.com/wormstest/src_vayu_windows/blob/main/2Poco X3 Pro Windows.png" width="350" alt="Windows 11 Running On A Poco X3 Pro">

# Windows en el POCO X3 Nfc

## Restaurar la tabla de particiones stock

### ¿Por qué lo necesitamos?

Si quieres desinstalar Windows usa esto para evitar el error humano evitar escribir una guia dedicada solo a desinstalar.

Si quieres blooquear tu bootloader de nuevo necesitas la tabla de particiones stock

### Requisitos Previos

- [gpt_both0.bin](../../../../releases/tag/binaries)

### Notes

> Reemplaza ```<gpt_both0.bin>``` por el directorio de gpt_both0.bin 


## Restaurar GPT

```cmd
fastboot flash partition:0 <gpt_both0.bin>
```

## Formatea userdata para evitar el bootloop y resturar el peso de FS
```cmd
fastboot -w
```
