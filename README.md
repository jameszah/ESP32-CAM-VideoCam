## ESP32-CAM-VideoCam

<a href="https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior">https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior</a>

You must have the Arduino IDE with the ESP32 boards library installed (giving you the ESP tools).
    
You also have to put your ESP32-CAM into programming mode (ground GPIO0 then power it on), and you must NOT have the Arduino Serial Monitor attached to the COM port.
    
You after have programmed the ESP32-CAM, you should get the config.txt file from here, open it with a text editor, and type in your ssid name and password, and then put that file onto an SD card and put it in the ESP32-CAM.  Then when you boot the ESP32-CAM it will connect to your network, and you can click its ip to do streaming, take a series of still pictures, download the movies you have recorded to your browser/computer, and edit the config.txt file to different framesizes, timelapses etc.


<br>
<br>
Click Connect to connect to ESP32-CAM and view console or send the firmware.    
<br>
<script  type="module" src="https://unpkg.com/esp-web-tools@7.0.0/dist/web/install-button.js?module"></script>
<esp-web-install-button manifest="manifest.json"></esp-web-install-button>
<br>    
Here is a link to the config.txt file you should save onto your sd card with your ssid and password.
<br>    
<a href="https://github.com/jameszah/ESP32-CAM-VideoCam/blob/main/config.txt">config.txt</a>
<br>
<br>

