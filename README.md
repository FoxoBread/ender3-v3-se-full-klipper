# ender3-v3-se-full-klipper - docker

[Klipper](https://github.com/Klipper3d/klipper) config for Creality Ender-3 V3 SE for running in docker.  
See https://github.com/mkuf/prind

For `CR4NS200320C13_32_MS35774_GD303RET6` mainboard (M4 label).


## Precompiled binaries
* `klipper.bin`   - serial over onboard USB type-C `(USART1 PA10/PA9)`.

Please note: I have not tried other serial connections.  
You are on your own for getting it to work with docker.

## Building Klipper from source and flashing
1. Clone the [base Klipper repository](https://github.com/Klipper3d/klipper).
2. `make menuconfig` and set options (see releases or top of `printer.cfg`.)
3. Place `klipper.bin` from `out/` in root of SD card.
4. Power on the printer and check for successful connection with controlling machine.

## Post installation steps:
1. Setting UDEV permissions correctly for serial port.
2. Bed mesh calibration
3. Manually calibrate Z-offset
4. Calibrate bed and extruder PID.
