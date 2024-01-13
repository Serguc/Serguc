# Use Github Action to compile Recovery
```
Support OFRP, SHRP, TWRP compilation and production
```
---

## Release Notes
```
= 2022/02/03
- Due to the hardware resource limitation of GitHub action, this version cannot be compiled based on AOSP and other source codes of Android 11 and above. If necessary, please use local compilation

= 2021/10/29: 
- Refactored version 2.0
- Completely reconstruct the use logic to reduce the difficulty of use
- Optimize the parameter transfer part, now you can run multiple Workers at the same time
- TWRP compilation test passed
- OFRP compilation test passed
- SHRP compile test passed
```

-----

## Parameter Description

| Name | Description | Example |
| ------------ | -------------------- | ------------ |
| `MANIFEST_TYPE` | Source Type | omni |
| `MANIFEST_URL` | Source address| [twrp-12.1](https://github.com/transsion-mt6789-recovery/twrp-device_infinix_Infinix-X6833B.git) |
| `MANIFEST_BRANCH` | Source branch | twrp-12.1|
| `DEVICE_TREE_URL` | Device address| twrp-12.1](https://github.com/transsion-mt6789-recovery/twrp-device_infinix_Infinix-X6833B.git) |
| `DEVICE_TREE_BRANCH` | Device branch | twrp-12.1 |
| `DEVICE_PATH` | Device location | Blackview Shark 8 |
| `DEVICE_NAME` | Shark 8 | Archytas |
repo init --depth=1 -u https://github.com/PitchBlackRecoveryProject/manifest_pb.git -b android-10.0
repo sync -j$(nproc --all) --force-sync
git clone https://github.com/OneGameKoTT/android_device_oukitel_c18pro-pbrp --depth=1 device/oukitel/c18pro
-----

## how to use
```
For example, your username is: Fun-114514
```
#### 1. Click'Fork' in the upper right corner of this warehouse
![](https://i.bmp.ovh/imgs/2021/10/6b6ed9f29e732372.png)
#### 2. After waiting for the automatic redirection, you will see your own username
![](https://i.bmp.ovh/imgs/2021/10/66cfe324c0ebb69b.png)
#### 3. Click'Actions-Make Recovery'
![](https://i.bmp.ovh/imgs/2021/10/23896d1b66292047.png)
#### 4. Click'Run workflow' and fill in according to the above'parameter description'
![](https://i.bmp.ovh/imgs/2021/10/9cb7871267cf2f53.png)
#### 5. After filling in, click'Run workflow' to start running

-----

## Compilation results
Can be downloaded at [Release](../../releases)

-----
## Remark

#### TeamWin Recovery Project: https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git
#### OrangeFox Recovery Project: https://gitlab.com/OrangeFox/Manifest.git
#### SKYHAWK Recovery Project: https://github.com/SHRP/platform_manifest_twrp_omni.git
