# Manual OC settings (advanced)

You can apply overclocking (OC) settings by manually changing the parameters in the **_device_settings.json_** file. This file is generated after the first successful boot on your mining rig and is saved on NiceHash OS bootable USB flash drive.  After that you can open _device_settings.json_ file and change power (TDP) settings, core and memory clocks for every device and algorithm separately.

```json
tdp: "default"
core_clocks: "default"
memory_clocks: "default"
```

## TDP (valid for both NVIDIA and AMD)
TDP is set as a percentage parameter for both NVIDIA and AMD graphics cards. If you want to change TDP you have to change the “default” state.

For example, if you want to change the TDP to 85% then you have to change it to ```“85”```.

For example, if you want to change the TDP to 110%, then you have to change it to ```“110”```.

## Core_clocks & memory_clocks (NVIDIA)
If you want to change core and memory clocks for **NVIDIA graphics cards** you have to take the “default” state as a base point.

For example, if you want to raise your core or memory clock for 50 Hz then you have to enter: ```“50”```.

For example, if you want to lower your core or memory clock for 50 Hz then you have to enter: ```“-50”```.

## Core_clocks & memory_clocks (AMD)
If you want to change core and memory clocks for **AMD graphics cards** you have to take the “default” state as a current clock state.

For example, if you want to raise your core or memory clock from 1800 to 1850 Hz then you have to enter ```“1850”```.

For example, if you want to lower your core or memory clock from 1800 to 1750Hz then you have to enter ```“1750”```.

## Algorithm IDs
In the table below you can find IDs for every algorithm:

| Algorithm        |ID|
|------------------|--|
| Scrypt           | 0|
| SHA256           | 1|
| ScryptNf         | 2|
| X11              | 3|
| X13              | 4|
| Keccak           | 5|
| X15              | 6|
| Nist5            | 7|
| NeoScrypt        | 8|
| Lyra2RE          | 9|
| WhirpoolX        |10|
| Qubit            |11|
| Quark            |12|
| Axiom            |13|
| Lyra2REv2        |14|
| ScryptJaneNf16   |15|
| Blake256r8       |16|
| Blake256r14      |17|
| Blake256r8vnl    |18|
| Hodl             |19|
| DaggerHashimoto  |20|
| Decred           |21|
| CryptoNight      |22|
| Lbry             |23|
| Equihash         |24|
| Pascal           |25|
| X11Gost          |26|
| Sia              |27|
| Blake2s          |28|
| Skunk            |29|
| CryptoNightV7    |30|
| CryptoNightHeavy |31|
| Lyra2Z           |32|
| X16R             |33|
| CrpytoNightV8    |34|
| SHA256AsicBoost  |35|
| Zhash            |36|
| Beam             |37|
| GrinCuckaroo29   |38|
| GrinCuckatoo31   |39|
| Lyra2REv3        |40|
| MTP              |41|
| CrpytoNightR     |42|
| CuckoCycle       |43|
