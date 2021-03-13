TWRP Device Tree for Cubot Note PLUS
===========
Unoffical Build for MT6737T TWRP 
------------------

Compiling on Ubuntu 20.10
```
repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

repo sync -c

git clone https://github.com/seluce/android_twrp_device device/CUBOT/NOTE_PLUS -b note-plus

. build/envsetup.sh

lunch omni_NOTE_PLUS-eng

export LC_ALL=C

mka recoveryimage
```

- full stable recovery twrp image (3.18.35)

Kernel patching was done following the tutorial from SachinBorkar by olt78 (Android-Hilfe.de)
https://forum.hovatek.com/thread-27132.html
Thanks a lot for your fantastic guide!
