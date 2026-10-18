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

## Boards (30)

| Board | Sensor | DRC errors / unconnected / parity |
|---|---|---|
| [S3 A1324](boards/a1324/) | Allegro A1324 low-noise linear Hall sensor | 0 / 0 / 0 |
| [S3 A3214](boards/a3214/) | Allegro A3214 micropower omnipolar Hall switch | 0 / 0 / 0 |
| [S3 ADS1115](boards/ads1115/) | TI ADS1115 16-bit 4-channel ADC | 0 / 0 / 0 |
| [S3 ADXL343](boards/adxl343/) | ADI ADXL343 3-axis accelerometer | 0 / 0 / 0 |
| [S3 ADXL345](boards/adxl345/) | ADI ADXL345 3-axis accelerometer | 0 / 0 / 0 |
| [S3 AH1806](boards/ah1806/) | Diodes AH1806 omnipolar Hall switch | 0 / 0 / 0 |
| [S3 AS5600](boards/as5600/) | ams AS5600 12-bit magnetic angle sensor | 0 / 0 / 0 |
| [S3 BNO055](boards/bno055/) | Bosch BNO055 9-axis absolute orientation sensor | 0 / 0 / 0 |
| [S3 BPW34S](boards/bpw34s/) | Osram BPW34S silicon photodiode light sensor | 0 / 0 / 0 |
| [S3 DRV5055](boards/drv5055/) | TI DRV5055 ratiometric linear Hall sensor | 0 / 0 / 0 |
| [S3 ICM-20602](boards/icm20602/) | TDK ICM-20602 6-axis IMU | 0 / 0 / 0 |
| [S3 ICM-20948](boards/icm20948/) | TDK ICM-20948 9-axis IMU | 0 / 0 / 0 |
| [S3 ICM-42688](boards/icm42688/) | TDK ICM-42688-P high-precision 6-axis IMU | 0 / 0 / 0 |
| [S3 IIM-42652](boards/iim42652/) | TDK IIM-42652 industrial 6-axis IMU | 0 / 0 / 0 |
| [S3 KX022](boards/kx022/) | Kionix KX022-1020 3-axis accelerometer | 0 / 0 / 0 |
| [S3 LIS2DH12](boards/lis2dh12/) | ST LIS2DH12 ultra-low-power 3-axis accelerometer | 0 / 0 / 0 |
| [S3 LIS2HH12](boards/lis2hh12/) | ST LIS2HH12 3-axis accelerometer | 0 / 0 / 0 |
| [S3 LIS2MDL](boards/lis2mdl/) | ST LIS2MDL 3-axis magnetometer | 0 / 0 / 0 |
| [S3 LIS3MDL](boards/lis3mdl/) | ST LIS3MDL 3-axis magnetometer | 0 / 0 / 0 |
| [S3 LSM6DS3](boards/lsm6ds3/) | ST LSM6DS3TR-C 6-axis IMU | 0 / 0 / 0 |
| [S3 LSM6DSL](boards/lsm6dsl/) | ST LSM6DSL 6-axis IMU | 0 / 0 / 0 |
| [S3 LSM6DSOX](boards/lsm6dsox/) | ST LSM6DSOX 6-axis IMU with machine-learning core | 0 / 0 / 0 |
| [S3 MPU6050](boards/mpu6050/) | InvenSense MPU-6050 6-axis IMU | 0 / 0 / 0 |
| [S3 SM351LT](boards/sm351lt/) | Honeywell SM351LT nanopower magnetoresistive switch | 0 / 0 / 0 |
| [S3 SS49E](boards/ss49e/) | SS49E linear Hall effect sensor | 0 / 0 / 0 |
| [S3 TLV493D](boards/tlv493d/) | Infineon TLV493D 3D magnetic sensor | 0 / 0 / 0 |
| [S3 TMAG5111](boards/tmag5111/) | TI TMAG5111 2D Hall latch (rotary encoder sensor) | 0 / 0 / 0 |
| [S3 VL53L0X](boards/vl53l0x/) | ST VL53L0X 2 m time-of-flight distance sensor | 0 / 0 / 0 |
| [S3 ToF](boards/vl53l1x/) | VL53L1X 4 m time-of-flight distance sensor | 0 / 0 / 0 |
| [S3 VL53L4CD](boards/vl53l4cd/) | ST VL53L4CD 1.3 m time-of-flight distance sensor | 0 / 0 / 0 |

**Not fabricated, assembled or powered.** Every number in a board's README is measured by KiCad 10 on the files in its folder (`report.json`); parts carry LCSC numbers and were in JLCPCB's stock on the date each README gives.

Each board folder holds `kicad/` (project), `fab/` (Gerbers zip, BOM, CPL, STEP, schematic PDF), `media/` (renders) and `board.json` (the brief it was generated from).

Designed with the HeyPCB method on KiCad 10 by heypcb-kicad's headless pipeline with Freerouting 2.4.1.

## Licence

CERN-OHL-S-2.0, © 2026 heypcb.ai. See [LICENSE](LICENSE).
