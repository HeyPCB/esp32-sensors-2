# HeyPCB ESP32-S3 Sensors 2: Motion, Magnetic, Sound & Power

ESP32-S3 boards, one sensor each: IMUs, accelerometers, magnetometers, Hall and angle sensors, microphones, distance, touch, optical and current monitors. KiCad 10, JLCPCB-ready, CERN-OHL-S-2.0.

Every board is the same ESP32-S3 template with one sensor: ESP32-S3-WROOM-1-N16R8 (16 MB flash, 8 MB PSRAM, Wi-Fi + Bluetooth LE), USB-C with native USB and an ESD clamp, an AP2112K 3.3 V LDO, BOOT and RESET buttons, power and user LEDs; 30 x 48 mm, 4 layers.

| Wiring | ESP32-S3 pin |
|---|---|
| I2C SDA / SCL | IO8 / IO9 |
| Sensor interrupt | IO7 |
| Analog in | IO1 (ADC1 channel 0) |
| SPI SCK / MOSI / MISO / CS | IO12 / IO11 / IO13 / IO10 |
| Digital / 1-Wire / PDM | IO4, IO5, IO6 |
| User LED | IO48 |

## Boards (8)

| Board | Sensor | DRC errors / unconnected / parity |
|---|---|---|
| [S3 ADXL343](boards/adxl343/) | ADI ADXL343 3-axis accelerometer | 0 / 0 / 0 |
| [S3 KX022](boards/kx022/) | Kionix KX022-1020 3-axis accelerometer | 0 / 0 / 0 |
| [S3 LIS2MDL](boards/lis2mdl/) | ST LIS2MDL 3-axis magnetometer | 0 / 0 / 0 |
| [S3 LIS3MDL](boards/lis3mdl/) | ST LIS3MDL 3-axis magnetometer | 0 / 0 / 0 |
| [S3 LSM6DS3](boards/lsm6ds3/) | ST LSM6DS3TR-C 6-axis IMU | 0 / 0 / 0 |
| [S3 MPU6050](boards/mpu6050/) | InvenSense MPU-6050 6-axis IMU | 0 / 0 / 0 |
| [S3 TLV493D](boards/tlv493d/) | Infineon TLV493D 3D magnetic sensor | 0 / 0 / 0 |
| [S3 ToF](boards/vl53l1x/) | VL53L1X 4 m time-of-flight distance sensor | 0 / 0 / 0 |

**Not fabricated, assembled or powered.** Every number in a board's README is measured by KiCad 10 on the files in its folder (`report.json`); parts carry LCSC numbers and were in JLCPCB's stock on the date each README gives.

Each board folder holds `kicad/` (project), `fab/` (Gerbers zip, BOM, CPL, STEP, schematic PDF), `media/` (renders) and `board.json` (the brief it was generated from).

Designed with the HeyPCB method on KiCad 10 by heypcb-kicad's headless pipeline with Freerouting 2.4.1.

## Licence

CERN-OHL-S-2.0, © 2026 heypcb.ai. See [LICENSE](LICENSE).
