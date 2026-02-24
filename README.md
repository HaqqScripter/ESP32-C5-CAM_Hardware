# ESP32-C5-CAM_Hardware
This repository contains the ESP32-C5-CAM (including the MINI series) development board hardware. This includes schematics, PCB. All of these are open-sourced so you can tinker them.

## ESP32-C5-CAM Series List (Board Revision)
- ESP32-C5-CAM (Not available at the moment)
- ESP32-C5-CAM-MINI (BETA1)
- ESP32-C5-CAM-DEVKIT (BETA1)

## ESP32-C5-CAM Board Preview
- ESP32-C5-CAM-MINI
![alt text](/Board/ESP32-C5-CAM-MINI/Revisions/BETA1/ESP32-C5-CAM-MINI-BETA1-PCB_SampleImage_3D.png "ESP32-C5-CAM-MINI-BETA1")
- ESP32-C5-CAM-DEVKIT
![alt text](/Board/ESP32-C5-CAM-DEVKIT/Revisions/BETA1/ESP32-C5-CAM-DEVKIT-BETA1-PCB_SampleImage_3D.png "ESP32-C5-CAM-DEVKIT-BETA1")

## Notes
- This was made to connect with DVP cameras such as OV5640/OV3660 with the Parallel IO interface to allow reasonably faster frame captures at high resolutions than the SPI interface. Users can refer to `esp_cam_io_parl` on how it works.
- Due to the absence of the SDMMC (SDIO Host) protocol, the SD Card is routed via the Fast SPI interface, to avoid GPIO matrix delays and possibly allow up to 40MHz clock, providing faster write speeds than 26.67MHz.
