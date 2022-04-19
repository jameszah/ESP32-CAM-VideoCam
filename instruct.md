
#### Goto the github.io websire ... not github.com

<img src="./doc/Screenshot 2022-04-19 121554.jpg">

###  Wire up the ESP32-CAM Correctly

### Click the Connect button
 
<img src="./doc/Screenshot 2022-04-19 121621.jpg">

### If you see this, we cannot see your ESP32 on a com port

<img src="./doc/Screenshot 2022-04-19 121727.jpg"> 

### Click on the Correct Com port for your ESP32-CAM, and click Connect

<img src="./doc/Screenshot 2022-04-19 121754.jpg"> 

### You should see this, then hit Logs and Console 

<img src="./doc/Screenshot 2022-04-19 121815.jpg"> 

### You will get this black box, now power on the ESP32, and you get this Ready to Program line

There are three on them here due to awkward plugging

<img src="./doc/Screenshot 2022-04-19 122153.jpg"> 

### Hit the Back Button in lower right of Black Box, and click Install ESP32-CAM-Wideo-Recorder

### And hit Install at this prompt - your ESP32 will be erased and installed

<img src="./doc/Screenshot 2022-04-19 122347.jpg"> 


<img src="./doc/Screenshot 2022-04-19 122243.jpg"> 

<img src="./doc/Screenshot 2022-04-19 122250.jpg"> 

<img src="./doc/Screenshot 2022-04-19 122339.jpg"> 

<img src="./doc/Screenshot 2022-04-19 122402.jpg"> 

### Next, power off ESP32, remove the Gpio0 jumper, restart the Logs and Console, then power it on

1.  The first 6 lines are the standard boot message.
2.  The Program starts
3.  You have nothing in EPROM
4.  Mount the SD card, and you have no config.txt
5.  Create a config.txt, and display the parameters, ...

<img src="./doc/Screenshot 2022-04-19 123318.jpg"> 

### Slide down the the mouse scroll wheel

1.  More prarmeters
2.  The ssid1234 is the code for no-wifi
3.  Create log file on sd, with your camera name and #1 session
4.  Set up camera
5.  Check you have 4MB of psram
6.  Start camera and print out type - ov2640 is the standard camera 
7.  Create some buffers
8.  Delete the oldest files if your sd is 80% full
9.  Start the camera and sd taks
10.  Start recording the movie
11.  It is desklens1.001.txt or camera name, session #1, movie #1

<img src="./doc/Screenshot 2022-04-19 123313.jpg"> 


<img src="./doc/Screenshot 2022-04-19 121727.jpg"> 
<img src="./doc/Screenshot 2022-04-19 121727.jpg"> 

