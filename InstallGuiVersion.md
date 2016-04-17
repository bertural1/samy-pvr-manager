# Introduction #

You can use the PVR Manager with or w/o SamyGO.
Without SamyGO you need Linux. Plug your pvr drive directly into your computer.

# Installation #

Download the program with your web browser.

## Run the program ##
### Linux ###
```
java -jar ~/Download/SamyPvrManager-X.xx.jar```

### Windows ###
Double click the SamyPvrManager-X.xx.jar file.

### To rename or delete titles ###
You need **write access** to folders CONTENTS and database
```
sudo chmod a+rw /media/your-pvr-volume/CONTENTS /media/your-pvr-volume/database```

## Known Bugs ##
### Windows ###
On **Windows 7 and Java 7** there is an problem with the IPv6 stack.
You'll get "CONTENTS not found".

To solve this you can:
  * add a firewall exception for the Java binary
  * run with -Djava.net.preferIPv4Stack=true (which disables IPv6)
  * or disable stateful FTP inspection in the firewall

```
netsh advfirewall set global StatefulFTP disable```
### Ubuntu ###
With Ubuntus default theme you cant see the menus.
There are two solutions:
  * Use another theme of Ubuntu
  * Use "Samy PVR Managers" alternative style (Options > Nimbus Style)