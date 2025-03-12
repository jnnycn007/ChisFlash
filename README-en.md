# ChisFlash
- ChisFlash is an open source GBA flashcart, which is inspired by the [opencartgba](https://github.com/laqieer/opencartgba) project.
- oshwhub(Latest version of PCB): [ChisBread](https://oshwhub.com/chisbread/works)
- v1.0(Prometheus) version uses FRAM, v0.1 version uses SRAM (1Mbit).

# Features

- The development goal of ChisFlash is to implement a fully functional GBA flashcart.

| Feature | Status |
| --- | --- |
| 256Mbit Flash | ✅ |
| 512Kbit SRAM/FRAM | ✅ |
| 1Mbit SRAM/FRAM (Bank Switching) | ✅ |
| 1Mbit/512Kbit Flash（Bank Switching） | ✅ |
| Real-Time Clock (RTC) | x |
| Rumble | x |
| Gyro | x |
| Solar Sensor | x |

# Images
![realcart](./images/realcart.png)
![top_v1.0](./images/top_v1.0.png)
![but_v1.0](./images/but_v1.0.png)
![top_v0.1](./images/top_v0.1.png)
![but_v0.1](./images/but_v0.1.png)

# Schematic

![schematic](./images/sch.png)

# BOM

- [ChisFlash BOM](BOM.md)

# Directory Structure   

```
ChisFlash
├── README.md
├── LICENSE
├── hardware
├── firmware
│   └── QuartusII1MSRAM
│   └── QuartusII1MFRAM
│   └── QuartusII1MFlash
├── document-zh
```

#### p.s.

- ChisFlash/hardware PCB design files
- ChisFlash/firmware/QuartusII1MSRAM is a CPLD/FPGA project for memory mapping (for 1M SRAM) [PCB,BOM](https://oshwhub.com/chisbread/chisflash-pichu)
- ChisFlash/firmware/QuartusII1MFRAM (for 1M FRAM) [PCB,BOM](https://oshwhub.com/chisbread/chisflash-prometheus)
- ChisFlash/firmware/QuartusII1MFlash (for 1M/512Kbit Flash) [PCB,BOM](https://oshwhub.com/chisbread/chisflash-celebi) [512Kbit ROM patch](https://github.com/ChisBread/gba-auto-batteryless-patcher/tree/custom_flashid)
- ChisFlash/document is a Chinese document for ChisFlash
