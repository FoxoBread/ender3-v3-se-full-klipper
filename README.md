# ender3-v3-se-full-klipper - docker

Klipper config and setup for Creality Ender-3 V3 SE under docker.  
See https://github.com/mkuf/prind

For `CR4NS200320C13_32_MS35774_GD303RET6` mainboard (M4 label).


## Precompiled binaries
* klipper12_type_c.bin   - for connection via type-c connector (USART1 PA10/PA9).
* klipper12_LCD_connector.bin  - for connection via IDC 10 pin LCD connector (USART3 PB11/PB10).

Please note: I have not tried the LCD binary. You are on your own for getting it to work with docker.

## Post installation steps:
1. Setting UDEV permissions correctly for serial port.
2. Bed mesh calibration
3. Manually calibrate Z-offset
4. Calibrate bed and extruder PID.
