# Z_Motion

[Z_Motion](https://6tron.io/z_object/z_motion_1_0_0) board support for Zephyr OS.

## Supported Features

The Zephyr Z_Motion board configuration supports the following hardware features:

| Interface  | Controller                                                                                        | Driver/Component     |
| :--------- | :------------------------------------------------------------------------------------------------ | :------------------- |
| AES        | on-chip                                                                                           | crypto               |
| CLOCK      | on-chip                                                                                           | clock_control        |
| DIE_TEMP   | on-chip                                                                                           | sensor               |
| DMA        | on-chip                                                                                           | dma                  |
| EXTI       | on-chip                                                                                           | interrupt_controller |
| FLASH      | on-chip                                                                                           | flash                |
| GPIO       | on-chip                                                                                           | gpio                 |
| I2C        | on-chip                                                                                           | i2c                  |
| PINCTRL    | on-chip                                                                                           | pinctrl              |
| RNG        | on-chip                                                                                           | entropy              |
| TIMER      | on-chip                                                                                           | counter, pwm, timer  |
| USBOTG_FS  | on-chip                                                                                           | usb                  |
| WWDG       | on-chip                                                                                           | watchdog             |
| SENSOR     | [BME280](https://www.bosch-sensortec.com/products/environmental-sensors/humidity-sensors-bme280/) | bme280               |
| SENSOR     | [BNO055](https://www.bosch-sensortec.com/products/smart-sensors/bno055/)                          | Not supported        |
| FUEL_GAUGE | [MAX17201](https://www.maximintegrated.com/en/products/power/battery-management/MAX17201.html)    | Not supported        |

See [Nordic vendor bindings](https://docs.zephyrproject.org/latest/build/dts/api/bindings.html#dt-vendor-nordic) for additional information.

## Usage

1. Add the Z_Motion board to your workspace using the [6TRON module](https://github.com/catie-aq/zephyr_6tron-manifest.git).
2. Compile and flash application using `west` tool:
   - Board name: `z_motion`
