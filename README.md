TeamWin Recovery Project

Device configuration for Nubia Z17 Mini (nx569j / nx569h)
=====================================

Basic   | Spec Sheet
-------:|:-------------------------
CHIPSET | Qualcomm MSM8976 Snapdragon 652 / Qualcomm MSM8976Pro Snapdragon 653
CPU     | Quad-core 1.4 GHz Cortex-A53 & Quad-core 1.8 GHz Cortex-A72 <br/> Quad-core 1.4 GHz Cortex-A53 & Quad-core 2.0 GHz Cortex-A72
GPU     | Adreno 510
Memory  | 4/6 GB
Shipped Android Version | Android 6.0 with Nubia UI
Storage | 64/128 GB
Battery | 2950 mAh (non-removable)
Dimensions | 146.7 x 72.5 x 7.5 mm (5.78 x 2.85 x 0.30 in)
Display | 1080 x 1920 pixels 5.2"
Rear Camera  | Dual 13.0 MP
Front Camera | 16.0 MP
Release Date | April 2017

<p align="center"><img src="https://forum.turkdevs.com/IMG/Nubia_Z17_Mini.jpg" alt="Nubia Z17 Mini" /></p>


## How-to compile it:

Add to `.repo/local_manifests/nx569j.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/nubia/nx569j" name="android_device_nubia_nx569j" remote="TeamWin" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_nx569j-eng
make -j$(nproc) recoveryimage
```