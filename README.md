## Flash Forge Creator Pro plugin for Cura

<img src="https://github.com/rubinlinux/FlashforgeCreatorProCura/assets/1413897/dde47608-0bc8-49b8-9fd9-9fae480d1c71" alt="screenshot showing the ffcp build plate in cura" width="200"/>

### ** This is a work in progress **

How to have the best experience with a Flashforge Creator Pro and Cura:

  * Get a raspberry pi, and install octopi or octoprint, hook it up to your Creator pro with a VERY HIGH QUALITY USB CABLE. Thick and short.
  * Install the GPX 2.6.8 plugin in octoprint
  * Install the X3GWriter plugin in Cura
  * Install this plugin in Cura
    * Check out or copy this repository's root directory as "FlashforgeCreatorproIntegration"  in your Cura plugins/ folder
      * On linux this is .local/share/cura/<version>/plugins/
      * On mac this is /Users/<you>/Library/Application Support/cura/<version>/plugins/
      * On win this is %appdata%\Roaming\cura\<version\plugins
      * so for example .local/share/cura/5.4/plugins/FlashforgeCreatorproIntegration/Installer.py ... etc
  * Once this plugin is installed, you should be able to find the Flashforge Creator Pro in the add printers list.
  * Go to the printer management screen and connect it with octoprint using an API key
  * You may need some consideration to which nozzle(s) you are using, can disable one maybe if not using it to avoid heating it up. (More documantation needed)


## Extruders
If using only SINGLE nozzle, please DISABLE UNUSED EXTRUDER before slicing to avoid heating up both nozzles and printing brim/skirt/raft with a different extruder! When using dual extrusion it's recommended to use ooze shield. Also use prime tower for the cleanest result, but it will significantly increase printing time and result in many tool changes due to dual extrusion implementation in Cura.

Remember - Extruder 1 is RIGHT, Extruder 2 is LEFT!

(In flashforge's internal parlance, the left extruder is 1, and the right one is 0)

BEFORE SLICING, DISABLE UNUSED EXTRUDER if using just one nozzle!

Remember, that that extruder 1 is right and extruder 2 is left. The easiest way to disable/enable specific extruder is to go to Settings menu and do it from there as they are named properly in it.


## Thanks To

This plugin is mainly https://github.com/eugr/Flashforge-for-Cura/ adapted to cura 5's new plugin format. Thanks to https://github.com/ronoaldo/FlashforgeFinderIntegration/ for some code & examples as well.
