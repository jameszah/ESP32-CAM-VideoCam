##  Lengthy Instructions to Install and Operate ESP32-CAM-VideoCam


## Goto the github.io website ... not github.com

<img src="./doc/Screenshot 2022-04-19 121554.jpg">

##  Wire up the ESP32-CAM Correctly

FTDI - ESP32   
Gnd  - Gnd   
TX   - UOR   
RX   - UOT   
+5   - +5   
   
When programming, jumper gpio0 to gnd (next pin)

Nice grapics from Dronebot 
https://dronebotworkshop.com/esp32-cam-microsd/

<img src="https://i0.wp.com/dronebotworkshop.com/wp-content/uploads/2022/04/esp32-cam-ftdi.jpg">

I have slightly different FTDI module - "shorter wires = fewer brownouts"    
If you use a breadboard or long USB cable you will get brownouts on the ESP32.  
Another solution is thick wires with nice soldering, and a 100 microFarad capactor between +5 and GND on ESP32  

Make sure FTDI has jumper set to 3.3v data for the ESP32 pins

GND - RX - TX in sequence

<img src="./doc/ftdi.jpg">

GND - UOT - UOR in sequnce, giving us the RX-UOT flip, and jumper on GND-Gpio0

<img src="./doc/esp32.jpg">

Plug in +5 to start in program mode

<img src="./doc/program.jpg">

Unplug +5, remove GND-Gpio0 jumper, put power back, and we are running!

<img src="./doc/run.jpg">



## Click the Connect button
 
<img src="./doc/Screenshot 2022-04-19 121621.jpg">

## If this box is empty, we cannot see your ESP32 on a com port

Make sure the com port is free -- not connected to arduino console for example

<img src="./doc/Screenshot 2022-04-19 121727.jpg"> 

## Click on the Correct Com port for your ESP32-CAM, and click Connect

<img src="./doc/Screenshot 2022-04-19 121754.jpg"> 

## You should see this, then hit Logs and Console 

<img src="./doc/Screenshot 2022-04-19 121815.jpg"> 

## You will get this black box, now power on the ESP32, and you get this Ready to Program line

There are three on them here due to awkward plugging

<img src="./doc/Screenshot 2022-04-19 122153.jpg"> 

## Hit the Back Button in lower right of Black Box, and click Install ESP32-CAM-Wideo-Recorder

## And hit Install at this prompt - your ESP32 will be erased and installed

<img src="./doc/Screenshot 2022-04-19 122347.jpg"> 


<img src="./doc/Screenshot 2022-04-19 122243.jpg"> 

<img src="./doc/Screenshot 2022-04-19 122250.jpg"> 

<img src="./doc/Screenshot 2022-04-19 122339.jpg"> 

<img src="./doc/Screenshot 2022-04-19 122402.jpg"> 

## Next, power off ESP32, remove the Gpio0 jumper, restart the Logs and Console, then power it on

1.  The first 6 lines are the standard boot message.
2.  The Program starts
3.  You have nothing in EPROM
4.  Mount the SD card, and you have no config.txt
5.  Create a config.txt, and display the parameters, ...

<img src="./doc/Screenshot 2022-04-19 123318.jpg"> 

## Slide down the the mouse scroll wheel

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
11.  It is desklens1.001.avi or camera name, session #1, movie #1

<img src="./doc/Screenshot 2022-04-19 123313.jpg"> 

## Accidently unplug the +5 volt wire

1.  You will see this on the console.
2.  This console only seems to update with a blank line
3.  You will see a line every 100 frames to show you progress with some nice stats
4.  And another line on an individual frame with more stats

<img src="./doc/Screenshot 2022-04-19 123428.jpg"> 

## Edit in your SSID and Password

1.  Since we screwed up the first recording, use this opportunity to pull out the sd, put it in your computer, and edit the config.txt on the sd card
2.  These are the files for the first session - the config.txt, the one movie, and the log file for the session.
3.  They have no dates because with no wifi, we do not know the date
4.  You can also add your timezone, and parameters or recording to realtime, timepalse, streaming speed, etc as described in config.txt file
5.  Make sure there are 2 spaces after the number or text, and before the // comment

<img src="./doc/Screenshot 2022-04-19 123308.jpg">

<img src="./doc/Screenshot 2022-04-19 123256.jpg"> 

## Now put the sd back in ESP32 and starts Logs and Console, and power up

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

##  Now look at Router to see your ESP32-CAM

This is how it looks on mine

<img src="./doc/Screenshot 2022-04-19 124039.jpg"> 

## Go to a browser on computer or phone and enter the name or ip of ESP32-CAM

<img src="./doc/Screenshot 2022-04-19 124045.jpg"> 

### And you get some stats

<img src="./doc/Screenshot 2022-04-19 124051.jpg"> 

## If you use Windows Chrome, you might get this ... Switch to Windows Edge

There is a bugfix to allocate more cookie buffers in ESP32 core

<img src="./doc/Screenshot 2022-04-19 125118.jpg"> 

## You can click the IP to update the stats, and you get his on console 

The http index line ... use this to force console to update

<img src="./doc/Screenshot 2022-04-19 124647.jpg"> 

## Try the Streaming on browser, and stats on console

1.  You get cosole messages when streaming begins and ends. 
2.  The console shows it is recording at 12.5 fps (the camera max), but streaming fluxuates a little from 15 down to about 12.

<img src="./doc/Screenshot 2022-04-19 124635.jpg"> 

<img src="./doc/Screenshot 2022-04-19 124652.jpg"> 

## Try the 10 photos at intervals - you can save these with your browser

<img src="./doc/Screenshot 2022-04-19 125104.jpg"> 

## Try the File Manager

These are your files from session #1 and #2 ... with dates

<img src="./doc/Screenshot 2022-04-19 125031.jpg"> 

## Click the filename to download it to your browser computer

These mjpeg avi's are big files - not enough ram or cpu time in a ESP32 to compact them.  
The ESP32 wifi is about 3.5 Mega-bits-per-second, and in a house with your router 50 feet away, you can get 3 Mbps when you are not recording, or about 2 Mbps when recording, with the on-module antenna.  Moving outside you will get slower speeds, and may need an external antenna.

But when you pull out the sd card, and plug it into your computer, you can copy the movies at about 20 Mega-bytes-per-second, or about 80 times faster than the transfer or wifi option.  Plus if you are recording, and doing a full speed file transfer, you will really burn out your battery, and heat up the ESP32, so ... it is of modest benefit, unless your camera is remote.  The wifi is very good for configuration, looking through the viewfinder, and occasionally grabbing a short avi.  I'm working on a version to hop around inside a movie to see if there is anything worth copying to the computer, without downloading the entire thing.
 
The file will land in your default download directory -- here it is one my Windows computer

<img src="./doc/Screenshot 2022-04-19 125037.jpg"> 

<img src="./doc/Screenshot 2022-04-19 132302.jpg"> 

## Click the "E" beseide config.txt to edit the config file

After you save the new config, you have to click "End Movie and Reboot" for it to take effect

<img src="./doc/Screenshot 2022-04-19 125111.jpg"> 

<img src="./doc/Screenshot 2022-04-19 125049.jpg"> 

## Start vlc on computer, Open a Network Stream

<img src="./doc/Screenshot 2022-04-19 125901.jpg"> 

## Enter the url from the Stream link on website and select Convert

<img src="./doc/Screenshot 2022-04-19 125855.jpg"> 

## Select Dump Raw Output, Browse to a FileName

<img src="./doc/Screenshot 2022-04-20 102421.jpg"> 

## Choose a computer file name to record the video stream, hit Save

<img src="./doc/Screenshot 2022-04-19 125849.jpg"> 

## and hit Start

The recording will be a mjpeg file, which has no sense of time, it just plays the stream as fast as it can.

<img src="./doc/Screenshot 2022-04-19 125831.jpg"> 

## hit the square stop button to stop streaming, and stream record


## When the sd video recording is done, you see some stats on the console, and in the log file

<img src="./doc/Screenshot 2022-04-19 130740.jpg"> 

## Now unplug everything, and put sd card in computer, and here are the movies

<img src="./doc/Screenshot 2022-04-19 131032.jpg"> 

## Any movie that does not end gracefully will not have an index, so vlc will show this, and it will not play at correct speed or length

<img src="./doc/Screenshot 2022-04-19 132316.jpg"> 

Here you are 44 seconds into a 21 second movie, from the unplug 5v incident - the movie has no index

<img src="./doc/Screenshot 2022-04-19 132247.jpg"> 

## The sd recorded movie, looks like the stream and computer recorded movie

<img src="./doc/Screenshot 2022-04-19 131254.jpg"> 

<img src="./doc/Screenshot 2022-04-19 131210.jpg"> 

## Questions, Comments, Like and Subscribe ...

## Other Programs in the ESP32-CAM-Video Recorder Family

https://github.com/jameszah/ESP32-CAM-Video-Recorder-junior   
- the source code for this program

https://github.com/jameszah/ESP32-CAM-Video-Recorder    
- older version, that will send photos and links to telegram.org at the end of every movie, and let you download that movie.
- has some PIR controls as well

https://github.com/jameszah/ESP32-CAM-Video-Telegram
- this will record photos or realtime/timelapse movies in memory and send the photo or movie to a telegram.org bot.
- you can use your telegram app on phone or copmputer to request a photo/movie, or have it triggered by a pir or radar module.
- No sd card required for this app, all the output is sent to telegram


## Are you still reading this?

I need a coffee!  Documentation is exhausting.

<https://ko-fi.com/jameszah>


