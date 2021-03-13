TWRP Device Tree for Cubot Rainbow
===========
Unoffical Build for MT6580 TWRP 
------------------

Compiling on Ubuntu 20.10
```
repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-6.0

repo sync -c

git clone https://github.com/seluce/android_twrp_device device/CUBOT/Rainbow -b rainbow

. build/envsetup.sh

lunch omni_Rainbow-eng

export LC_ALL=C

mka recoveryimage
```

- full stable recovery twrp image (3.18.19)
