# Nintendo Switch Guides
This repository is a ground for all my Nintendo Switch guides, so that anyone can view and consume them. 

## Disclaimer
The content in these guides is provided for informational purposes only, and I do not take any responsibilty should you damage your device while attempting to follow any instructions on this page. Proceed at your own risk.

## Table of Contents
1. Overview
2. Updating your Custom Firmware (CFW)
3. Booting to CFW
4. Updating your Switch's Firmware
5. Updating Homebrew Apps
6. Installing NSPs through USB

## 1. Overview
This guide assumes you already have a hacked or hackable Switch. For more information on performing the hack, see [this guide](https://switch.homebrew.guide/).

## 2. Updating your CFW
To update your CFW, you need to perform the following steps:
1. Download the latest Atmosphere ZIP file from [here](https://github.com/Atmosphere-NX/Atmosphere/releases).
2. (Optional) Download any sigpatches you may need. You can search Google for these and just drop them onto the root of your SD card (and overwrite the existing contents).
3. (Optional) Download the latest version of [hekate](https://github.com/CTCaer/hekate/releases). Copy the ```bootloader``` folder from this ZIP file to the root of your SD card (and overwrite the existing contents). Copy the ```hekate_ipl.ini``` file from this repo to the ```/bootloader``` folder on your SD card.

## 3. Booting to CFW
1. Download [TegraRCMGUI](https://github.com/eliboa/TegraRcmGUI/releases).
2. Download either the [hekate](https://github.com/CTCaer/hekate/releases) payload or the [fusee-primary](https://github.com/Atmosphere-NX/Atmosphere/releases) payload.
3. Connect your Switch via regular USB and put your Switch into RCM. Follow [this guide](https://switch.homebrew.guide/gettingstarted/checkingrcm) to do so.
4. Open TegraRCMGUI and select either the hekate BIN file or the fusee-primary BIN file you downloaded from above. Click the ```Inject payload``` button.
5. Your Switch should automatically boot to the Atmosphere CFW. If it does not, try to inject the other payload. If this fails also, then you will have to revisit the section above and make sure all steps were followed properly.

## 4. Updating your Switch's Firmware
To update your CFW, you will need to perform the following steps:
1. Download [ChoiDujourNX](https://switchtools.sshnuke.net)  (it's a homebrew app) and copy the NRO file from the ZIP file to the ```/switch``` folder on your SD.
2. Find the firmware file you want from [here](https://darthsternie.net/switch-firmwares). Create a new folder in the root of your SD card named ```/firmware```. Unzip the firmware files to ```/firmware/<version>``` on your SD card.
3. Boot up Atmosphere and go to the homebrew launcher. You can do this by holding ZR and selecting the Album icon. Then launch ChoiDujourNX (it looks like a rabbit icon).
4. Click on the firmware folder, then the ```<version>``` folder, then hit ```Choose``` at the bottom. Wait for it to finish. Then click on the version name with exFAT. Wait for it to finish. Then click on ```Start installation```. Wait for it to finish.
5. Reboot and profit.

## 5. Updating Homebrew Apps
To update any Homebrew apps, you will need to copy the respective NRO file to the ```/switch``` folder on your SD card, and overwrite the existing contents.

## 6. Installing NSPs through USB
Follow [this guide](https://switch.homebrew.guide/usingcfw/installnsps/installnsps-nsusbloader).
