# android-hosts-file-adblocking-script
 * Reqirements:
  - Root
  - a recent busybox version. (Usually included in most custom ROMs)

 * Usage:
  - Open a shell on your phone. (adb shell, or terminal emulator)
  - Dowload ```gethosts```
  - Install the script in /system/bin so the script can be made executable
    - Remount /system read/write: ```mount -o rw,remount /system```
    - Copy ```gethosts``` to ```/system/bin/gethosts``` 
    - Remount /system read only: ```mount -o ro,remount /system```
    
  - Run ```gethosts``` as root to download and install or update the hosts-file 
  
  
  The script will backup your old hostsfile on /sdcard/hosts.BAK
  
  
  Remember that running scripts as root from strangers can be dangerous!
 




Loosely based on https://wiki.ubuntuusers.de/hosts/
