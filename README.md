# LeEco Le Pro 3 Dolby Atmos
This module enables LeEco Le Pro 3 Dolby Atmos port and is the second most compatible of all the ports. [More details in support thread](https://forum.xda-developers.com/android/software/soundmod-axon-7-dolby-atmos-t3412342).

### Dependencies
* [Audio Modification Library](https://forum.xda-developers.com/apps/magisk/module-audio-modification-library-t3579612) @ XDA Developers

## Compatibility
* Android Marshmallow+
* init.d (LineageOS SU, phh's SU, & rootless)
* MagiskSU & SuperSU
* Magisk & System install
* Nexus/Pixel support (A/B OTA)
* SELinix enforcing (LOS SU & rootless need permissive)
* Works with [AM3D Zirene Sound](https://forum.xda-developers.com/android/apps-games/mod-zirene-sound-am3d-t3396698/post71580634#post71580634} & ViPER4Android [FX](https://forum.xda-developers.com/apps/magisk/module-viper4android-fx-2-5-0-5-t3577058)/XHiFi

## Change Log
v3.0
	- Unity/AML v2.0: Massive installer and script overhaul
	- Unity v2.0: Added autouninstall (if mod is already installed and you flash same version zip again, it'll uninstall), thus removing the need for an uninstall zip
	- Unity v2.0: Added file/folder backup/restore of modified files
	- Unity v2.0: Added file/folder backup/restore of normally wiped files
	- Unity v2.0: Added Osm0sis @ xda-developers uninstaller idea (just add "uninstall" to zip name and it'll function as uninstaller)
	- Unity/AML v2.0: Added phh's SuperUser and LOS su support (note, LOS doesn't support sepolicy patching)
	- Unity/AML v2.0: Added proxy library to AML to allow the proxy effects found in multiple audio modules
	- Unity/AML v2.0: Added support for Magisk imgs located in /cache/audmodlib
	- Unity v2.0: Added system_root support for Pixel devices
	- Unity v2.0: Added system override (if you're on magisk but would rather have it install to system, add word "system" to zip name and it'll install everything but scripts to system)
	- Unity v2.0: Add Unity system props
	- Unity v2.0: Added vendor fix for Nexus devices
	- Unty/AML v2.0: AML functionality and uses overhauled
	- Unity/AML v2.0: Bug fixes
	- Unity/AML v2.0: Modified Unity Installer to allow use for non AML modules
	- Unity/AML v2.0: Moved scripts from Magisk .core to the individual module folder due to .core limitations
	- Unity/AML v2.0: New modular approach - no need to modify update-binary anymore: check instructions for more details on how this works
	- Unity v2.0: Reworked addon.d system install scripts
	- Unity/AML v2.0: Removed AML cache workaround by reworking AML changes via magisk_merge
	- Unity/AML v2.0: Reworked AML vendor audio_effects to not be overwritten by system audio_effects by commenting out conflicting lines
	- Unity v2.0: Reworked script permissions
	- Unity/AML v2.0: Update sepolicy for Magisk 13+
	- Unity/AML v2.0: Updated to Magisk module template 1400

v2.4
	- AudModLib v1.4 update which changes SELinux live patching to allow better compatibility between different devices, kernels, and roms; while also keeping the amount of "allowances" to a minumum
	- AudModLib v1.4: changed post-fs-data(.d)/service(.d) shell script names for cosmetic recognition
	- AudModLib v1.4: merge SuperSU shell script with MagiskSU post-fs-data(.d) script for less fragmentation
	- AudModLib v1.4: added /cache/audmodlib.log to determine if script has run successfully
	- AudModLib v1.4: more audio policy files and various mixer_paths files are now included in the framework
	- Install script changes that include: major update to Pixel (A/B OTA) support, mounting changes, improved script efficiency, fixes & consolidation, and cosmetic fixes
	- Add/fix proper addon.d support

v2.3
	- AudModLib v1.3 update push which includes the script addition to allow various audio mods working with SELinux Enforcing
	- Remove (audmodlib)service.sh and replace with post-fs-data(.d) audmodlib.sh, which should fix when root may be lost upon installing certain mods
	- Remove force SELinux Permissive post-fs-data script "setenforce 0"
	- System install will now have the same script updates as the AudModLib v1.3 to allow to work in SELinux Enforcing

v2.2
	- Added audmodlib.sh post-fs-data.d script
	- Install script fixes
	- post-fs-data.d script fixes
	- Push AudModLib v1.2 hotfixes

v2.1
	- AudModLib v1.1 hotfix for bootloops issues on some devices

v2.0
	- Initial Magisk release

## Credits
* [Dolby Laboratories](https://www.dolby.com/us/en/brands/dolby-atmos.html)
* [LeEco](http://www.leeco.com/us/)

## Source Code
* Module [GitHub](https://github.com/therealahrion/Dolby-Atmos-LeEco-Le-Pro-)
* Collective Dolby Atmos Ports [GitHub](https://github.com/therealahrion/Collective-Dolby-Atmos-Ports)
