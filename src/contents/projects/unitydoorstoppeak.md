---
title: Unity Doorstop Peak
description: UnityDoorstop fork that's specfically tailored for the game PEAK. It offers a signature-based in-memory patch to the UnityPlayer to bypass the -force-vulkan parameter. This aims to replace https://github.com/CyR1en/UnityPlayerPatcher but essentially has the same inner working. So if you want to know more about how this works, you can read about it over there. Additional configuration is added for flexibility (see configuration below).
poster: /projects/generic.webp
techstack:
  - CPP
---

UnityDoorstop fork that's specfically tailored for the game PEAK. It offers a signature-based in-memory patch to the UnityPlayer to bypass the -force-vulkan parameter. This aims to replace [UnityPlayerPatcher](https://github.com/CyR1en/UnityPlayerPatcher) but essentially has the same inner working. So if you want to know more about how this works, you can read about it over there.
[[source](https://github.com/CyR1en/UnityDoorstop-PEAK)]

### Additional Configuration:
```ini
[Extra]

# If true, UnityPlayer will be patched to bypass force vulkan.
bypass_vulkan=false
```

### Additional CLI Argument
| Argument                                          | Description                                                                                          |
| ------------------------------------------------- |------------------------------------------------------------------------------------------------------|
| `--doorstop-bypass-vulkan bool`                   | If true, UnityPlayer will be patched to bypass force vulkan.                                         |