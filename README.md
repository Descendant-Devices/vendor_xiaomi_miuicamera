Copyright (C) 2020 Carlos Ayrton Lopez Arroyo (Official-Ayrton990)

Copyright (C) 2020 ANXCamera by AEonAX

MiuiCamera from ANXCamera
=========================================

This repository can be used to ship Xiaomi's MiuiCamera app ported from the ANXCamera's Magisk module on custom A11 ROMs. The APK has been manually patched to make the majority of functions to work perfectly on lmi/umi/cmi/cas/apollopro. Some blobs has been updated from V12.2.4.0.RJKMIXM

## Currently supported devices:
* Xiaomi Mi 10 family (umi/cmi/cas)
* Xiaomi POCO F2 Pro (lmi, lmipro)
* Xiaomi Mi 10T Pro  (apollo/apollopro)

## How to build?

- Simply on you device.mk inherit the repo by: `$(call inherit-product-if-exists, vendor/xiaomi/miuicamera/config.mk)`
- It's adviced to include sepolicy even if you are not running enforced system, include sepolicy on your BoardConfig.mk by: `-include vendor/xiaomi/miuicamera/BoardConfigVendor.mk`
- Clone this repo following the path: `rom-source/vendor/xiaomi/miuicamera`

## Bugs:

- Portrait mode crashing (if triggered, clean data and follow next step again)
- It needs to grant manually all permissions requiered to avoid force close
- Wide angle seems to be not working
