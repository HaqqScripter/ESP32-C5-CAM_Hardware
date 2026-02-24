# ESP32-C5-CAM_Hardware
This repository contains the ESP32-C5-CAM (including the MINI series) development board hardware. This includes schematics, PCB. All of these are open-sourced so you can tinker them.

## Notes
- This was made to connect with DVP cameras such as OV5640/OV3660 with the Parallel IO interface to allow reasonably faster frame captures at high resolutions than the SPI interface. Users can refer to `esp_cam_io_parl` on how it works.
- The SD Card is routed via the Fast SPI interface, to avoid GPIO matrix delays and possibly allow up to 40MHz clock, providing faster write speeds.
