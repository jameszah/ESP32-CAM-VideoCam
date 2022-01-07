
## https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior

<a href="https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior"></a>
    
Click here [https://jameszah.github.io/ESP32-CAM-VideoCam/flash.html]  to install a video recorder on on ESP32-CAM module.  
    
    <a href="https://jameszah.github.io/ESP32-CAM-VideoCam/flash.html"></a>
    
You must have the ESP tools installed, or just the Arduino IDE with the ESP32 boards library installed (giving you the ESP tools).
    
You also have to put your ESP32-CAM into programming mode (ground GPIO0 then power it on), and you must not have the Arduino Serial Monitor attached to the COM port.
    
You after have programmed the ESP32-CAM, you should get the config.tx file from here, open it with a text editor, and type in your ssid name and password, and then put that file onto an SD card and put it in the ESP32-CAM.  Then when you boot the ESP32-CAM it will connect to your network, and you can click its ip to do streaming, take a series of still pictures, download the movies you have recorded to your browser/computer, and edit the config.txt file to different framesizes, timelapses etc.
   
