# `HowTo` label your PVR disk #

If you want to give your PVR disk a better label than 31a77b-42d...
you can do this with the following commands


## Run in terminal ##

  * Unmount your PVR disk (e.g. /dev/sdc)
```
sudo umount /dev/sdc```
  * Label it with xfs\_admin (e.g. PVR)
```
sudo xfs_admin -L PVR /dev/sdc```