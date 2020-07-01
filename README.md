# Solution

#   Linux Mint Ulyana(20)

1. Linux Mint 20 Blocks Snap App Installs. "package 'snapd' has no installation candidate error".

    Solution: sudo rm /etc/apt/preferences.d/nosnap.pref
 
2. Linux Mint - No Bluetooth adapters found

   Solution: You could try blacklisting one bluetooth module and then load it later to see if there is some firmware loading issue
             CODE: 
             echo "blacklist btusb" | sudo tee /etc/modprobe.d/btusb.conf
             Reboot, wait 15 seconds after everything is loaded and in terminal

             sudo modprobe btusb
             See if you have better result
             
 3. Run apps on a hardware device Linux
    Solution: The following example shows how to install the Android adb tools package.

              apt-get install adb
