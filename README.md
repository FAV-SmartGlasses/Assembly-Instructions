# Assembly Instructions

## Hardware
- Download and print our model ([Model STL](URL Placeholder))
- Buy the components from the table bellow
 
| Component                           | Usage       | URL                                                                                                                                                                                                                                                                                                                                                                    | 
|-------------------------------------|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Display                             | **AR & VR** | https://rpishop.cz/lcd-oled-displeje/1405-waveshare-55-hdmi-amoled-displej-1920x1080-kapacitni.html                                                                                                                                                                                                                                                                    | 
| Cardboard glasses (only for lenses) | **AR & VR** | https://allegro.cz/nabidka/vr-bryle-portsmouth-hnede-14829232993?utm_feed=712e6653-4749-4512-b084-b6e297fc9e0b&utm_source=google&utm_medium=cpc&utm_campaign=CZ%3EGeneral%3EFallback%3E3P%3EPLA&ev_adgr=Fallback%3E3P%3EPLA&ev_campaign_id=20077339122&gad_source=1&gclid=Cj0KCQiAwOe8BhCCARIsAGKeD57zpy058x9i49HOO94Y7X7ohtmadU0cYYqpkUCx-0ZiWQQhzD1qHeEaAsiAEALw_wcB |
| Raspberry                           | **AR & VR** | https://rpishop.cz/raspberry-pi-5/6497-raspberry-pi-5-4gb-ram.html                                                                                                                                                                                                                                                                                                     |
| BNO055 IMU sensor                   | **VR**      | https://e-shop.prokyber.cz/vstupni/adafruit-9-dof-bno055/?srsltid=AfmBOorPTSj2cIcaWKYosiWsK5Ili8ADpRpDdVgcaO730ql-ODoFyF9N                                                                                                                                                                                                                                             |
| Passive cooling case                | **AR & VR** | https://rpishop.cz/541270/edatec-hlinikovy-case-s-pasivnim-chladicem-pro-raspberry-pi-5-cerny-ed-picase-ob/                                                                                                                                                                                                                                                            |
| micro-HDMI -> HDMI Cable            | **AR**      | https://rpishop.cz/micro-hdmi/1867-raspberry-pi-microhdmi-kabel-1-m-cerna.html                                                                                                                                                                                                                                                                                         |
| Camera                              | **AR**      | https://rpishop.cz/mipi-kamerove-moduly/5600-raspberry-pi-camera-module-3-wide.html                                                                                                                                                                                                                                                                                    |
| Camera cable                        | **AR**      | https://rpishop.cz/mipi/6501-raspberry-pi-5-camera-cable-standard-mini-200-mm.html                                                                                                                                                                                                                                                                                     |
| Power bank                          | **AR & VR** | https://www.alza.cz/epico-multiportova-powerbanka-20-100mah-bila-d7899089.htm#parameters                                                                                                                                                                                                                                                                               |

## Basic setup

1. Swap the camera cable - the default one isn't compatible with RPI 5
2. Mount the cooling case and connect the camera to the CSI port

## IMU sensor setup

| IMU pin | RPI pin                                  |
|---------|------------------------------------------|
| `3V`    | `3.3V`                                   |
| `GND`   | `GND`                                    |
| `SCL`   | `SCL`                                    |
| `SDA`   | `SDA`                                    |
| `ADR`   | `GND`                                    |
| `PS0`   | `GND`                                    |
| `PS1`   | `GND`                                    |
| `RST`   | `3.3V` or `GND` - Connect it to a button |