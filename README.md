# Nintendo Switch Guides
This repository is a ground for all my Nintendo Switch guides, so that anyone can view and consume them. 

## Disclaimer
The content in these guides is provided for informational purposes only, and I do not take any responsibilty should you damage your devices while attampting to follow any instructions on this page. Proceed at your own risk.

## Table of Contents
1. Overview
2. Updating your Custom Firmware (CFW)
3. Updating your Switch's Firmware
4. Updating Homebrew Apps

## 1. Overview
This guide assumes you already have a hacked or hackable Switch. For more information on performing the hack, see [this guide](https://switch.homebrew.guide/).

## 2. Updating your CFW
To update your CFW, you need to perform the following steps:
1. Download the latest Atmosphere ZIP and BIN files from [here](https://github.com/Atmosphere-NX/Atmosphere/releases).
2. (Optional) Download any sigpatches you may need. You can search Google for these and just drop them onto the root of your SD card (and overwrite the existing contents).
3. (Optional) Download the latest version of [hekate](https://github.com/CTCaer/hekate/releases). Copy the ```bootloader``` folder from this ZIP file to the root of your SD card (and overwrite the existing contents). Copy the ```hekate_ipl.ini``` file from this repo to the ```/bootloader``` folder on your SD card.

## 3. Updating your Switch's Firmware
To update your CFW, you will need to perform the following steps:
1. Download [ChoiDuJourNX](https://switchtools.sshnuke.net)  (it's a homebrew app) and copy the NRO file from the ZIP in the ```/switch``` folder on your SD.
2. Find the firmware file you want from [here](https://darthsternie.net/switch-firmwares). Create a new folder in the root of your SD card named ```/firmware```. Unzip the firmware files to ```/firmware/<version>``` on your SD.
3. Boot up CFW and go to the homebrew launcher. You can do this by holding ZR and selecting the Album icon. Then launch ChoiDuJourNX (it looks like a rabbit icon).
4. Click on the firmware folder, then the ```<version>``` folder, then hit ```Choose``` at the bottom. Wait for it to finish. Then click on the version name with exFAT. Wait for it to finish. Then click on ```Start installation```. Wait for it to finish.
5. Reboot and profit.

## 4. Updating Homebrew Apps
To update any Homebrew apps, you will need to copy the respective NRO file to the ```/switch``` folder on your SD card, and overwrite the existing contents.
