<p align="center"><img src="https://github.com/K3V1991/Install-ADB-and-Fastboot-on-Android-Devices/blob/main/Command.png" width="200"></a>
<h1 align="center"><b>Learn how you can execute ADB and Fastboot Commands on Android Phone and Tablet Devices</b></h1>
<br />

## NFO:
ADB and Fastboot have become essential Tools for every Developer and advanced Android User nowadays. 
One of the main Advantages of using ADB or Fastboot in you can install System Updates, Custom ROMs, Boot Images, Custom Kernel and Applications as well.
Let's say that your PC isn't working or maybe you are traveling and the PC available doesn't have ADB/Fastboot installed.
This Guide here will show you how to install ADB and Fastboot on any Android Smartphone or Tablet, so can perform all the Activities you would on your PC.

## Requirements:
* Rooted Android Phone or Tablet
* [Termux](https://play.google.com/store/apps/details?id=com.termux) or [Terminal Emulator for Android](https://play.google.com/store/apps/details?id=jackpal.androidterm) 
* Root Explorer App (e.g: Root Explorer, Es File Explorer, MiXplorer)
* [ADB and Fastboot Binaries](https://github.com/dingyi222666/termux-sdk-tools) thanks to [dingyi222666](https://github.com/dingyi222666)
* OTG Cable (Make sure that your Device supports OTG)
<br />

**[List of ADB and Fastboot Commands](https://github.com/K3V1991/ADB-and-FastbootPlusPlus/blob/main/Commands.txt)**
<br />
<br />

## Copy Binary Files to Device:
* Root Explorer: Extract the downloaded ADB and Fastboot Files and copy the Contents to /system/bin Folder

or

* Terminal:
1. Download and extract the ADB and Fastboot Files on the Device (e.g: /sdcard/Download/)
2. Install and launch a Terminal App, type the following Commands in sequence:
```
su 
```  
Gains Root Priviledges
```                              
cd /sdcard/Download 
```
Changes the working Directory to Download Folder
```
mount -o remount,rw /system   
```
Remounts the System Partition
```
cp adb /system/bin/adb
```
```
cp fastboot /system/bin/fastboot 
```
Copys the adb and fastboot Files to the bin Folder

## Make the Files executable:
```
chmod 755 /system/bin/adb
``` 
```
chmod 755 /system/bin/fastboot
```
3. Type: ```su```, connect another Device using a OTG Cable and use ADB and Fastboot Commands

## Screenhot:
<img src="https://github.com/K3V1991/Install-ADB-and-Fastboot-on-Android-Devices/blob/main/Termux-adb.jpg" width="300"></a>
