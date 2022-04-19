
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

### Accidently unplug the +5 volt wire

1.  You will see this on the console.
2.  This console only seems to update with a blank line
3.  You will see a line every 100 frames to show you progress with some nice stats
4.  And another line on an individual frame with more stats

<img src="./doc/Screenshot 2022-04-19 123428.jpg"> 

### Edit in your SSID and Password

1.  Since we screwed up the first recording, use this opportunity to pull out the sd, put it in your computer, and edit the config.txt on the sd card
2.  These are the files for the first session - the config.txt, the one movie, and the log file for the session.
3.  They have no dates because with no wifi, we do not know the date
4.  You can also add your timezone, and parameters or recording to realtime, timepalse, streaming speed, etc as described in config.txt file
5.  Make sure there are 2 spaces after the number or text, and before the // comment

<img src="./doc/Screenshot 2022-04-19 123308.jpg">

<img src="./doc/Screenshot 2022-04-19 123256.jpg"> 

### Now put the sd back in ESP32 and starts Logs and Console, and power up

1.  You will see these 3 screens 
2. Reboot message
3. You now have Eprom, so goto next session #2
4. Mound sd card, and get your new config and display

<img src="./doc/Screenshot 2022-04-19 123839.jpg"> 

1.  Create a new log file for session #2
2.  Connect to wifi - print out the names to make sure they are correct
3.  Get the date and time
4.  Print the ip address
5.  Regisiter your name "desklens" with your router
6.  Set up camera


<img src="./doc/Screenshot 2022-04-19 123846.jpg"> 

1.  Start recording desklens2.001.avi

<img src="./doc/Screenshot 2022-04-19 123852.jpg"> 

###  Now look at Router to see your ESP32-CAM

This is how it looks on mine

<img src="./doc/Screenshot 2022-04-19 124039.jpg"> 

### Go to a browser on computer or phone and enter the name or ip of ESP32-CAM

<img src="./doc/Screenshot 2022-04-19 124045.jpg"> 

### And you get some stats

<img src="./doc/Screenshot 2022-04-19 124051.jpg"> 

### If you use Windows Chrome, you might get this ... Switch to Windows Edge

<img src="./doc/Screenshot 2022-04-19 123256.jpg"> 

### You can click the IP to update the stats, and you get his on console 

The http index line ... use this to force console to update

### Try the Streaming on browser, and stats on console

<img src="./doc/Screenshot 2022-04-19 124647.jpg"> 

<img src="./doc/Screenshot 2022-04-19 124635.jpg"> 

<img src="./doc/Screenshot 2022-04-19 124652.jpg"> 


