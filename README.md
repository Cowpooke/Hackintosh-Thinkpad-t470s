# Hackintosh-Thinkpad-t470s

[![macOS](https://img.shields.io/badge/macOS-Ventura-orange)](https://www.apple.com/macos/ventura/)
[![OpenCore](https://img.shields.io/badge/OpenCore-1.0.2-blue)](https://github.com/acidanthera/OpenCorePkg)

</br>

| Model              | Lenovo ThinkPad T470s                                                                              |
|:-------------------|:----------------------------------------------------------------------------------------------------------|
| Processor          | Intel Core i5-7300U (2C, 4T,  2.6GHz / 2.71GHz) vPro                                                              
| Graphics           | Integrated Intel HD 620 Graphics                                                                         |
| Memory             | 8 GB DDR4 (1x 4 GB DDR4 SODIMM + 1x 4 GB SODIMM)                                                       |
| Display            | 14" HD (1920x1080), Non-Touch                                                                      |
| Storage            | 256 GB SATA SSD                                                                                  |

</br>

## What working:
- Intel HD 620 Graphics
- Fan control with yogaSMC
- Power management (CPU friend data)
- Wi-Fi
- Dual Battery (combined to 1 battery)
- Apple HD Audio (layout id = 29)
- HDMI

## Issue
- audio jack sometimes distorted, go to system-settings -> sound -> input to fix the audio

## Post Install
Disable hibernation, since it doesn't work properly on hackintoshes
```
sudo pmset autopoweroff 0
sudo pmset powernap 0
sudo pmset standby 0
sudo pmset proximitywake 0
sudo pmset tcpkeepalive 0
```
