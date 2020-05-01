# Nintendo Switch Guides
This repository is a ground for all my Nintendo Switch guides, so that anyone can view and consume them. 

## Disclaimer
The content in these guides is provided for informational purposes only, and I do not take any responsibilty should you damage your device while attempting to follow any instructions on this page. Proceed at your own risk.

## Table of Contents
01. Getting Started
02. Booting to CFW
03. Configuring 90DNS
04. Starting the Homebrew Launcher
05. Updating Homebrew Apps
06. Updating your Custom Firmware (CFW)
07. Updating your Switch's Firmware
08. Installing NSPs through USB
09. Accessing SD Card Without Removing
10. Installing RetroArch
11. Running Content on Retroach

## 01. Getting Started
This guide assumes you already have a hacked or hackable Switch. For more information on performing the hack, see [this guide](https://switch.homebrew.guide/).

## 02. Booting to CFW
1. Download [TegraRCMGUI](https://github.com/eliboa/TegraRcmGUI/releases).
2. Download either the [hekate](https://github.com/CTCaer/hekate/releases) payload or the [fusee-primary](https://github.com/Atmosphere-NX/Atmosphere/releases) payload.
3. Connect your Switch via regular USB and put your Switch into RCM. Follow [this guide](https://switch.homebrew.guide/gettingstarted/checkingrcm) to do so.
4. Open TegraRCMGUI and select either the hekate BIN file or the fusee-primary BIN file you downloaded from above. Click the ```Inject payload``` button.
5. Your Switch should automatically boot to the Atmosphere CFW. If it does not, try to inject the other payload. If this fails also, then you will have to revisit the steps in this section and make sure all steps were followed properly.

## 03. Configuring 90DNS
The first thing you should do when booting CFW is to address the internet situation. You have two choices for setting up WiFi on your Switch while using CFW:
1. Don't connect to the internet at all. Always keep Airplane Mode on + Bluetooth for controllers. If you think there is risk of connecting accidentally, use the below option instead.
2. Keep WiFi on, but block any connections to Nintendo's servers. Follow [this guide](https://nh-server.github.io/switch-guide/extras/blocking_updates/) to set this up. This will reduce the risk of getting banned.

## 04. Starting the Homebrew Launcher
When starting the homebrew launcher or running any homebrew app, it is recommended to use Atmosphere's title override feature. Follow these steps:
1. Press and hold the R button on the controller. Keep holding it until you get to step 4.
2. Open any installed game on your Switch.
3. Wait until the homebrew launcher shows up.
4. Release the R button.

## 05. Updating Homebrew Apps
To update any Homebrew apps, you will need to copy the respective NRO file to the ```/switch``` folder on your SD card, and overwrite the existing contents.

## 06. Updating your CFW
To update your CFW, you need to perform the following steps:
1. Download the latest Atmosphere ZIP file from [here](https://github.com/Atmosphere-NX/Atmosphere/releases).
2. (Optional) Download any sigpatches you may need. You can search Google for these and just drop them onto the root of your SD card (and overwrite the existing contents).
3. (Optional) Download the latest version of [hekate](https://github.com/CTCaer/hekate/releases). Copy the ```bootloader``` folder from this ZIP file to the root of your SD card (and overwrite the existing contents). Copy the ```hekate_ipl.ini``` file from this repo to the ```/bootloader``` folder on your SD card.

## 07. Updating your Switch's Firmware
To update your CFW, you will need to perform the following steps:
1. Download [ChoiDujourNX](https://switchtools.sshnuke.net)  (it's a homebrew app) and copy the NRO file from the ZIP file to the ```/switch``` folder on your SD.
2. Find the firmware file you want from [here](https://darthsternie.net/switch-firmwares). Create a new folder in the root of your SD card named ```/firmware```. Unzip the firmware files to ```/firmware/<version>``` on your SD card.
3. Boot up Atmosphere and go to the homebrew launcher. You can do this by holding R and selecting any installed game. Make sure to hold the R button until the homebrew launcher comes up. Then launch ChoiDujourNX (it looks like a rabbit icon).
4. Click on the firmware folder, then the ```<version>``` folder, then hit ```Choose``` at the bottom. Wait for it to finish. Then click on the version name with exFAT. Wait for it to finish. Then click on ``Select firmware``. Wait for it to finish. Then click on ```Start installation```. Wait for it to finish.
5. Reboot and profit.

## 08. Installing NSPs through USB
Follow [this guide](https://switch.homebrew.guide/usingcfw/installnsps/installnsps-nsusbloader).

## 09. Accessing SD Card without Removing
1. Download the [NXMTP](https://github.com/liuervehc/nxmtp/releases) homebrew app.
2. Launch it on the Switch while it's plugged into your PC. You will then be able to access the SD card's contents as if it was plugged into the PC directly. Be aware that it will be slower though.

## 10. Installing RetroArch
1. Go to the [Retroarch download page](https://buildbot.libretro.com/stable/), find ```<latest version>/nintendo/switch/libnx``` and download ```RetroArch.7z```. You will need 7-Zip installed on your PC to extract this file.
2. Extract the archive to the root of your SD card to install or update your copy of RetroArch (overwrite any existing file).
3. Run Retroarch using one of two ways:
   
   (a) Atmosphere's title takeover feature (Hold R and launch any game; keep holding R until the homebrew menu shows up). Then launch Retroarch from there.
   
   (b) Install a [Forwarder NSP](https://mega.nz/#!WLwBAIiI!hfgcJdKA04gpmGlWc198tBba07AGUjryIYP0S8xtNJg) with Goldleaf and launch this instead. Note that the first method is recommended over this one, but I included it here for completeness.

## 11. Running Content on Retroach
Always use "unheadered" (or "no intro") files for Retroarch. If you see "[!]" in the file name or the ZIP file name, this will likely not run properly in Retroarch.
