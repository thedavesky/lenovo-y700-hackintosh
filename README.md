# Lenovo Y700 Hackintosh
![Release](https://img.shields.io/github/release/thedavesky/lenovo-y700-hackintosh.svg?style=flat-square)
![Repo size](https://img.shields.io/github/repo-size/thedavesky/lenovo-y700-hackintosh.svg?style=flat-square)
![Language count](https://img.shields.io/github/languages/count/thedavesky/lenovo-y700-hackintosh.svg?style=flat-square)
![Top language](https://img.shields.io/github/languages/top/thedavesky/lenovo-y700-hackintosh.svg?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/thedavesky/lenovo-y700-hackintosh.svg?style=flat-square)
![License](https://img.shields.io/github/license/thedavesky/lenovo-y700-hackintosh.svg?style=flat-square)
> A complete OpenCore EFI configuration for Lenovo Y700 to run a fully functional macOS operating system.

I have been using Lenovo Y700 as my daily driver since 2016. As of 2018, I am using macOS on this machine as my main system. MacOS runs on it very well and I don't have any crashes or freezes. But in 2021 it doesn't have enough power for my workload and I'm already tired of hackintoshing, so I'm planning switching to MacBook Pro with Apple Silicon at the end of this year.

## Configuration
|Specifications|Detail|
|-|-|
|Computer Model|Lenovo Y700-17ISK|
|Processor|Intel Core i7-6700HQ|
|Memory|16GB Kingston DDR4 2133MHz|
|Hard Disk|Samsung SSD 850 EVO M.2 250GB + WD Blue Slim 1TB|
|Integrated Graphics|Intel HD Graphics 530|
|Sound Card|Realtek ALC235|
|Wireless Card|Broadcom BCM94352Z|
|Touchpad|Synaptics PS2|

## Installation
- Set serial numbers in config.plist as per [OpenCore Install Guide](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html).
- Copy EFI folder to your EFI partition.
- Install macOS.
	- After installing macOS I recommend to configure [ALCPlugFix-Swift](https://github.com/black-dragon74/ALCPlugFix-Swift). Lenovo Y700 has a combo jack and macOS doesn't support it out of the box. Prepared configuration files for this program are already in this repository in a folder ALCPlugFix-Swift.

## Status
- **Discrete GPU** isn't working.
	- MacOS doesn't support Optimus technology. I disabled dGPU in BIOS settings.
- **Subwoofer** isn't working.
	- It isn't configured in AppleALC and macOS doesn't have native support for 2.1 audio.
- **SD Card Reader** isn't working.
- **Handoff** sometimes doesn't work as expected.
	- Broadcom BCM94352Z isn't fully compatible with macOS. I recommend using other wireless card.
- Everything else works well.

## Pictures
<div align="center">
    <a href="https://raw.githubusercontent.com/thedavesky/lenovo-y700-hackintosh/assets/images/workplace.jpg">
        <img src="https://raw.githubusercontent.com/thedavesky/lenovo-y700-hackintosh/assets/images/workplace.jpg" alt="Workplace">
    </a>
</div>
<div align="center">
    <a href="https://raw.githubusercontent.com/thedavesky/lenovo-y700-hackintosh/assets/images/about_this_mac.jpg">
        <img src="https://raw.githubusercontent.com/thedavesky/lenovo-y700-hackintosh/assets/images/about_this_mac.jpg" alt="About this mac">
    </a>
</div>

## Author
Copyright ⓒ 2021 Dawid Maliszewski (thedavesky) <dawid@thedavesky.com>

## License
This project is licensed under the **GNU General Public License v3.0** - see the [LICENSE](https://github.com/thedavesky/lenovo-y700-hackintosh/blob/master/LICENSE) file for details.
