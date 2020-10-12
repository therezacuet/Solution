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
            
# Runtime permissions
With API level >= 21, you will need to request runtime permissions to access the SD card, the camera, and other things.
              
  from android.permissions import request_permissions, Permission
request_permissions([Permission.WRITE_EXTERNAL_STORAGE])


https://medium.com/frontend-coach/angular-in-motion-4-approaches-to-animation-1aa7426aae5a

http://myhexaville.com/2018/04/30/flutter-canvas-animations/

Flutter web apps deploy to c-panel using node js
https://blog.logrocket.com/flutter-web-app-node-js/

https://connectwww.com/how-to-install-and-configure-apachephpmysql-and-phpmyadmin-on-ubuntu/727/


Linux Volume Increase command:
pactl set-sink-volume 0 180%

Web App deploy on shared hosting 
https://blog.logrocket.com/flutter-web-app-node

https://techviewleo.com/how-to-install-anydesk-on-linux-mint/

https://github.com/MahajanTarun/Pose-Estimation-Android-app-using-Deep-Learning


https://github.com/beraldofilippo/android-hpe-library
