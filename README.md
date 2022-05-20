## ESP32-CAM-VideoCam

If you are reading this on github.com, click here to read it on github.io -- the download controls only work on github.io
  
<a href="https://jameszah.github.io/ESP32-CAM-VideoCam/">https://jameszah.github.io/ESP32-CAM-VideoCam/</a>

<a href="https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior">https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior</a>

Here are some demo videos uploaded to Youtube - timelapse and realtime - see the "junior" link above for details:

[![Click to see on Youtube](http://img.youtube.com/vi/tzMFukXsX6o/hqdefault.jpg)](http://www.youtube.com/watch?v=tzMFukXsX6o "Clouds from Youtube")

[![Click to see on Youtube](http://img.youtube.com/vi/SNbKu3UN2P8/hqdefault.jpg)](http://www.youtube.com/watch?v=SNbKu3UN2P8 "Birds from Youtube")

### Lengthy Install and Operations Instructions here

<a href="https://jameszah.github.io/ESP32-CAM-VideoCam/instruct">https://jameszah.github.io/ESP32-CAM-VideoCam/instruct</a>

    
You also have to put your ESP32-CAM into programming mode (ground GPIO0 then power it on), and you must NOT have the Arduino Serial Monitor attached to the COM port.
    
After you have programmed the ESP32-CAM, you should get the config.txt file from here, open it with a text editor, and type in your ssid name and password, and then put that file onto an SD card and put it in the ESP32-CAM.  Then when you boot the ESP32-CAM it will connect to your network, and you can click its ip to do streaming, take a series of still pictures, download the movies you have recorded to your browser/computer, and edit the config.txt file to different framesizes, timelapses etc.


<br>
Click Connect to connect to ESP32-CAM and view console or send the firmware -- make sure Arduino serial monitor is closed!    
<br>
<script  type="module" src="https://unpkg.com/esp-web-tools@7.0.0/dist/web/install-button.js?module"></script>
<esp-web-install-button manifest="manifest.json"></esp-web-install-button>

<br>  

Here is a link to the **config.txt** file you should save onto your sd card with your ssid and password.  The link below has comments to describe the fields in greater detail, or cut-and-paste this little window for the basics.
<br>   
<br>
<a href="https://github.com/jameszah/ESP32-CAM-VideoCam/blob/main/config.txt">config.txt</a>
<br>

```
desklens  // camera name
11  // framesize  11=hd
1800  // length of video in seconds
0  // interval - ms between recording frames 
1  // speedup - multiply framerate 
0  // streamdelay - ms between streaming frames
GMT // timezone
ssid1234  // ssid wifi name
mrpeanut  // ssid password
```

***

### May 5, 2022 -- New Version 58.9 for    
1. esp32-arduino 2.0.3   
2. restore wifi when fails   
3. esp camera mod for CAMERA_GRAB_LATEST   
4. mods to allow streaming faster than recording   
5. correct 'Header fields are too long for server to interpret' bug

<script
  type="module"
  src="https://unpkg.com/esp-web-tools@8.0.1/dist/web/install-button.js?module"
></script>

<esp-web-install-button
  manifest="./v58.9/manifest.json"
></esp-web-install-button>

### May 19, 2022 -- New Version 59.5 for    
1. ap mode for controlling camera with router 
2. ... and setting ssid for router
3. ... and setting time when in ap mode
4. faster more effiecent streaming
5. more options for multi-photo command

<script
  type="module"
  src="https://unpkg.com/esp-web-tools@8.0.1/dist/web/install-button.js?module"
></script>

<esp-web-install-button
  manifest="./v59.5/manifest.json"
></esp-web-install-button>

Slightly different config file:
<a href="https://github.com/jameszah/ESP32-CAM-VideoCam/blob/main/v59.5/config.txt">config.txt</a>
