## Flash Forge Creator Pro plugin for Cura

### ** This is a work in progress **

How to have the best experience with a Flashforge Creator Pro and Cura:

  * Get a raspberry pi, and install octopi or octoprint, hook it up to your Creator pro with a VERY HIGH QUALITY USB CABLE. Thick and short.
  * Install the GPX 2.6.8 plugin in octoprint
  * Install the X3GWriter plugin in Cura
  * Install this plugin in Cura
    * Check out or copy this repository's root directory as "FlashforgeCreatorproIntegration"  in your Cura plugins/ folder
      * On linux this is .local/share/cura/<version>/plugins/
      * so .local/share/cura/5.4/plugins/FlashforgeCreatorproIntegration/Installer.py ... etc
  * Once this plugin is installed, you should be able to find the Flashforge Creator Pro in the add printers list.
  * Go to the printer management screen and connect it with octoprint using an API key
  * You may need some consideration to which nozzle(s) you are using, can disable one maybe if not using it to avoid heating it up. (More documantation needed)



## Thanks to

This plugin is mainly https://github.com/eugr/Flashforge-for-Cura/ adapted to cura 5's new plugin format. Thanks to https://github.com/ronoaldo/FlashforgeFinderIntegration/ for some code & examples as well.
