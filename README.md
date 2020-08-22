# Samsung M30 SM-M305[F]/[M] TWRP Device Tree

#Find kernel source over here https://github.com/akhil1999/android_kernel_samsung_m30lte

This branch is for building of TeamWin Recovey Project (TWRP) Recovery.
This tree compatible with TWRP 3.4.0.0, pie sources.

---
![Samsung Galaxy M30](https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-m30-sm-m305f-1.jpg)


# About Device

Samsung Galaxy M30 (m30lte)

### Specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 2x1.8GHz A73 + 6x1.6Ghz A53, ARM HMP big.LITTLE GTS
CHIPSET | Samsung Exynos 7904
GPU     | ARM Mali G71 MP2
Memory  | 3 GB / 4 GB / 6 GB
Shipped Android Version | 8.1.0
Updated Android Version | 10.0
Storage | 32 GB / 64GB / 128GB
MicroSD | Up to 64 GB
Battery | 5000 mAh (non-removable)
Dimensions | 159 x 75.1 x 8.5 mm
Display | 1080 x 2340 pixels, 6.4" Super AMOLED
Rear Camera  | 13.0 MP, 5 MP, 5 MP LED flash
Front Camera | 16.0 MP

---

#  Steps to Compile

 Add Omni Source or Minimal TWRP Source
 
 `repo sync git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0`
 
Then Run `repo sync` 

```sh
. source ./build/envsetup.sh && lunch omni_m30lte-userdebug && make clean && make -j# recoveryimage
```
`# = No. of CPU threads of your PC'

### Thanks to:
 * myself, akhil1999
 * TeamWin
