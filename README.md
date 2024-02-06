# VKD3Don7

VKD3Don7, a patch for [vkd3d-proton](https://github.com/HansKristian-Work/vkd3d-proton) ([2.6](https://github.com/HansKristian-Work/vkd3d-proton/releases/tag/v2.6)), provides support for the Windows® 7 operating system.

## Hardware Support & Requirements

All `NVIDIA` and `RADEON` graphics processors with `Vulkan 1.2` capabilities are supported, `RADEON` support being, albeit, tremendously experimental.

## Capabilities

Depending on program and hardware, performance can range from ~85% of native, to less than half. Stutters, graphical anomalies, a disproportional impact on performance caused by certain settings, random crashes and overall unexpected behavior may occur.

Implying, of course, the program starts at all. Generally, there are three types of program :

- Programs that require `DirectX® 12` :
	- These may work.

- Programs that require `DirectX® 12` and check for the current Windows® version :
	- These will not work. Spoofing the reported Windows® version may bypass this.

- Programs that require `DirectX® 12` and depend on libraries exclusive to Windows® 8, 8.1, 10 or 11 :
	- These will not work. Providing modified libraries may bypass this.

## Installation

VKD3Don7 requires the `dxgi.dll` from [dxvk](https://github.com/doitsujin/dxvk) ([1.10.3](https://github.com/doitsujin/dxvk/releases/tag/v1.10.3)). After procurement, the `d3d12.dll` from VKD3Don7, along with the `dxgi.dll` from [dxvk](https://github.com/doitsujin/dxvk) ([1.10.3](https://github.com/doitsujin/dxvk/releases/tag/v1.10.3)), need to be put into the directory of the programs executable file.