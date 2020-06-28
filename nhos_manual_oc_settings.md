# Manual OC settings (advanced)

You can apply overclocking (OC) settings by manually changing the parameters in the **_device_settings.json_** file. This file is generated after the first successful boot on your mining rig and is saved on NiceHash OS bootable USB flash drive.  After that you can open _device_settings.json_ file and change power (TDP) settings, core and memory clocks for every device and algorithm separately.

```json
tdp: "default"
core_clocks: "default"
memory_clocks: "default"
```

## TDP (valid for both NVIDIA and AMD)
TDP is set as a percentage parameter for both NVIDIA and AMD graphics cards. If you want to change TDP you have to change the ```“default”``` value.

For example, if you want to set TDP to 85% then you have to change this value to ```"tdp": 85```.

For example, if you want to set TDP to 110%, then you have to change this value to ```"tdp": 110```.

## Core_clocks & memory_clocks (NVIDIA)
If you want to change core and memory clocks for **NVIDIA graphics cards** you have to change the ```“default”``` value. Value is relative to card default value.

For example, if you want to raise your core or memory clock for 50 Hz then you have to change this value to ```"core_clocks": 50``` or ```"memory_clocks": 50```.

For example, if you want to lower your core or memory clock for 50 Hz then you have to change this value to ```"core_clocks": -50``` or ```"memory_clocks": -50```.

## Core_clocks & memory_clocks (AMD)
If you want to change core and memory clocks for **AMD graphics cards** you have to change the ```“default”``` value. Values for AMD cards are absolute.

For example, if you want to raise your core or memory clock from 1800 to 1850 Hz then you have change this value to ```"core_clocks": 1850``` or ```"memory_clocks": 1850```.

For example, if you want to lower your core or memory clock from 1800 to 1750 Hz then you have change this value to ```"core_clocks": 1750``` or ```"memory_clocks": 1750```.

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
| GrinCuckarood29  |44|
| Beamv2           |45|
| X16Rv2           |46|
| Eaglesong        |48|
| GrinCuckaroom29  |49|
| GrinCuckatoo32   |50|
| Handshake        |51|
| KAWPOW           |52|
| Cuckaroo29BFC    |53|
| BeamV3           |54|
