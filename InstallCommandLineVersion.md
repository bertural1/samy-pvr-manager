# Introduction #

All you need is a Linux system (e.g. Ubuntu). If you haven't any, you can use a bootable USB stick. There are many tutorials in the web to create a bootable USB stick. Make sure you have a little space left for the program.

# Installation #

  * First you should boot Ubuntu from your USB stick (or boot other Linux distro)
  * Download the program with your web browser
  * Start a terminal program
  * Copy the jar file to your home directory
```
cp ~/Download/samypvredit-05.jar ~/samypvredit.jar```

  * Connect your PVR disk to your computer

## Run the program ##
```
java -jar ~/samypvredit.jar```
You should see the usage screen:
```
Usage:
java -jar samypvredit.jar [-l] file|folder
java -jar samypvredit.jar -s file title [description]

Example:
java -jar samypvredit.jar -l /media/your-pvr-volume/CONTENTS```

### To list the PVR disk content ###
```
java -jar ~/samypvredit.jar -l /media/your-pvr-volume/CONTENTS```

### To rename the title ###
```
java -jar ~/samypvredit.jar -s /media/your-pvr-volume/CONTENTS/#number#.inf "New title"```
You need **write access** to folders CONTENTS and database
```
sudo chmod a+rw /media/your-pvr-volume/CONTENTS /media/your-pvr-volume/database```

### To set title and description ###
If you have a TV (D-Series?) with larger INF-files (7464 bytes) you can set the recording description
```
java -jar ~/samypvredit.jar -s /media/your-pvr-volume/CONTENTS/#number#.inf "New title" "New description"```