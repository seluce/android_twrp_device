TWRP Device Tree for Cubot X18
===========
Unoffical Build for MT6737T TWRP 
------------------

Compiling on Ubuntu 20.10
```
repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

repo sync -c

git clone https://github.com/seluce/android_twrp_device device/CUBOT/X18 -b x18

. build/envsetup.sh

lunch omni_X18-eng

export LC_ALL=C

mka recoveryimage
```

- full stable recovery twrp image (3.18.35)

Full working touchscreen in twrp! Kernel patching was done following the tutorial from SachinBorkar by seluce
