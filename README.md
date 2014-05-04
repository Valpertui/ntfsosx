ntfsosx
=======

Patched ntfs script to support drives with spaces in their names

Usage
=====

* Eject properly the device from a Windows computer.
* Plug the device on your mac
* Launch Terminal
* execute :
~~~
chmod +x ./ntfs.sh
sudo ./ntfs.sh
~~~

More
====

The device will not appear in the Finder
You can access it in (DeviceName is the name of your device, ex : "My Passport") `/Volumes/DeviceName`
~~~
open /Volumes/DeviceName
~~~
Will open a Finder window for the device
You can create a symbolic link to it on the desktop by doing : `ln -s /Volumes/DeviceName ~/Desktop/DeviceName`
If you want to remove the symlink : `rm -f ~/Desktop/DeviceName`
If you want to remove ntfs support : `sudo rm -f /etc/fstab`
