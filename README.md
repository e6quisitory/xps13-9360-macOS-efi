# XPS 13 9360 macOS EFI

| Info | Value |
| ------------- | ------------- |
| macOS Version  | 12.5 Monterey  |
| OpenCore Version | 0.8.2 |
| BIOS Version | 2.12|
| CPU  | Intel Core i5-7200U (Kaby Lake)  |
| iGPU | Intel HD Graphics 620 |
| RAM | 8 GB |
| Network/Bluetooth Card | BCM4352 |
| SSD | WD Black SN750 500 GB |

Refer to [this repo](https://github.com/theQuert/XPS-9360-macOS) for my BIOS settings; they're pretty much the same.

| Broken/Not Working | Info/Workaround |
| ------------------ | ---------- |
| Airdrop & Handoff | Airdrop from other device to XPS works fine, but reverse doesn't work.</br>Handoff works spottily sometimes, other times not at all. |
| Universal Control & Sidecar | I think the [FeatureUnlock](https://github.com/acidanthera/FeatureUnlock) kext is needed, which I have not added. |
| Hardware DRM</br>(Apple TV, Netflix & Amazon Prime in Safari don't play) | Use software DRM browser like Chrome |
| Brightness function keys | Use [MonitorControl](https://github.com/MonitorControl/MonitorControl) 
| USB-C/Thunderbolt | For USB-C, must properly map ports. Thunderbolt I disabled in BIOS. |
| Battery life | Greatly reduced vs Windows. Still lasts 3-4 hours, through, so it's satisfactory.</br>Perhaps caused due to running SSD in AHCI instead of RAID. [Optimization](https://dortania.github.io/OpenCore-Post-Install/universal/pm.html) is possible, however. I just did not bother as I normally use with AC adapter plugged in. |

Everything is working except the list above. Used this configuration for a year without any hiccups.</br>Have now switched to a 2012 MacBook Air. Spec downgrade, yes, however, dat Apple materials and build quality, and ergonomics, is just something else...
