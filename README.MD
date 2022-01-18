# Doogee X5 Max Pro
# About phone
!(https://manual-user-guide.com/images/phones/doogee_x5_max_pro.png)

_|_
------------ | -------------
CPU | MT6737m
RAM |  2 Gb
ROM | 16 Gb
Screen | 5", 720 x 1280, IPS
GPU | Mali-T720 MP1

# Drivers used
_|_
------------ | -------------
ALS/PS | EPL259X NEW
Accel |  KXTJ2 1009 NEW
Magnetometr | QMC6983 NEW
Fingerprint | MICROARRAY FP
LCM | otm1283a_cmi50_tps65132_hd
Touchscreen | Focaltech
Imgsensors | gc5024_mipi_raw gc5005_mipi_raw hi553_mipi_raw hi843b_mipi_raw hi841_mipi_raw mn045_mipi_raw hi544_mipi_raw
Charger | PMIC

#### Kernel source 3.18.19+ MT6737m
### Compiling

```sh
$ make O=out/Build ARCH=arm CROSS_COMPILE=(TOOLCHAIN arm-eabi 4.9-5.5) n370b_full_defconfig
$ make O=out/Build ARCH=arm CROSS_COMPILE=(TOOLCHAIN arm-eabi 4.9-5.5) -j* (*-threads)
$ . adb-push    <<< Connect phone to PC and use it. Reboot phone in recovery menu and flash file kernel(....).zip
```

--------------------------------------------------------------
Applyed patch "00_yy_patch" (fix build error for Ubuntu 21.10)
