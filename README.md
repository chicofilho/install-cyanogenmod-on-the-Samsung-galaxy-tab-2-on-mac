Installing cyanogenmod on the Samsung galaxy tab2 using Mac
=======================================================

Samsung devices come with a unique boot mode called Download Mode which is very similar to Fastboot Mode on some devices with unlocked bootloaders. Heimdall is a cross-platform, open source tool for interfacing with Download Mode on Samsung devices. The preferred method of installing a custom recovery is through this boot mode. Rooting the stock firmware is neither recommended nor necessary.

Download and install the <a href="http://glassechidna.com.au/heimdall/#downloads">Heimdall Suite</a>

* After installation, heimdall should be available from the terminal; type 'heimdall version' to verify installation succeeded.

* Download koush's ClockworkMod Recovery. You can directly download the recovery image using the link below, or visit clockworkmod.com/rommanager to check for the latest version (if your device can be found there). Be careful to select the right image!
** koush's ClockworkMod Recovery: <a href="http://download2.clockworkmod.com/recoveries/recovery-clockwork-6.0.2.3-p3100.img">recovery-clockwork-6.0.2.3-p3100.img
** md5: ff97383788b9a5da3cfa35e686a265c9

* The file may not be named identical to what's in the flash command below. If the file is wrapped in a zip or tar file, extract the file and flash that in the flashing step, heimdall does not care what the name is as long as you use the proper partition.

* Power off the Galaxy Tab 2 7.0 (GSM) and connect the USB adapter to the computer but not to the Galaxy Tab 2 7.0 (GSM), yet.

* Boot the Galaxy Tab 2 7.0 (GSM) into download mode by holding Volume Down & Power. Accept the disclaimer on the device. Then, insert the USB cable into the device.
At this point, familiarize yourself with the Flashing heimdall notes below so that you are prepared for any strange behavior if it occurs.

* On the computer, open a terminal (or Command Prompt on Windows) in the directory where the recovery image is located and type:
heimdall flash --RECOVERY recovery.img --no-reboot

* A blue transfer bar will appear on the device showing the recovery being transferred.
Unplug the USB cable from your device

* You can now manually reboot the phone into ClockworkMod Recovery mode by holding the turn on button.

* Download the prebuilt release of CyanogenMod you wish to install. (Or if you've built CM yourself, look in the $OUT directory for the .zip.)
Optional: Download any supplemental 3rd-party applications packages for the device you wish to use.
** Pass it to a micro sd card

