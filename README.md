# **soundtrack**
 * Released under GNU General Public Licence, V3.0 
 * Plays an area-themed soundtrack whilst you disc! Quality .wav files provided
 * **Prerequisite**: - you must have installed the [Quow minimap plugin](https://quow.co.uk/minimap.php)
 
A Plugin for the [DiscWorld MUD](http://discworld.starturtle.net/lpc/) - Play an area themed sound track whilst you disc!

**current version *v4.1***

#### by Mickey
#### based on the original 'soundtrack_v4.zip' by Kilstrin (quit)
---

## About
This is a [MUSHclient](http://www.gammon.com.au/mushclient/) plugin for the text-based [MUD Discworld](http://discworld.starturtle.net/lpc/), which is based upon the [Discworld series of novels](https://www.terrypratchettbooks.com/about-sir-terry) by celebrated [author Sir Terry Pratchett](https://www.terrypratchettbooks.com/book-series/discworld/).

This plugin requires functionality from [minimap](https://quow.co.uk/minimap.php), a rather excellent plugin by another disc mudder, [Quow](https://quow.co.uk/).* If you don't already have his plugins and related database, you are really missing out. You are either really old school - in which case, we salute you! - or you are a glutten for punishment and hard work, in which case, we salute you!

## Installing

1. Download the release (soundtrack.zip) file, and extract the content to your /plugins/ folder.
- When extracting, **keep the directory structure intact**, *otherwise you will need to edit **Soundtrack_v4.xml**, at line 662:*
  - Line 662: `SoundsFolder = GetPluginInfo(GetPluginID(), 20) .. "sounds\\"`
-- *By default, this would makes the sounds directory* C:\fromProgram Files\MUSHclient\plugins\sounds\

  Would become:
  - Line 662: `SoundsFolder = GetPluginInfo(GetPluginID(), 20) .. ""` (If the sounds are in the same directory as the script)

2. Open MUSHclient, and navigate to the plugins dialog box, **File -> Plugins** and click the Install button.
- - Navigate to the plugins folder (which should be being displayed as the default location unlesss you have changed the MUSHclient settings.
- - Select the **Soundtrack_v4.1.xml** file, and MUSH will do the rest!

#### Now your MUD immersion is complete with aural as well as visual stimulation!

## Using

The Soundtrack plugin will be enabled by default. You can display the various options and some about information for the plugin by typing:
- `help soundtrack`

You can turn the sounds on & off, as directed by the above help, by using `soundtrack on` and `soundtrack off`

`Soundtrack Plugin:
==================
 * by Mickey, based on soundtrack_v4.zip by Kilstrin (quit)
 * v.4.1 - https://github.com/nos78/soundtrack
'help soundtrack'            :  This help information
'soundtrack on'              :  Enables Soundtrack Plugin
'soundtrack off'             :  Disables Soundtrack Plugin
'soundtrack stop'            :  Stops all music currently playing
'soundtrack volume <x>'      :  Sets the decibel level of the plugin (more negative is quieter and more positive is louder)
'soundtrack current volume'  :  Displays current volume
'soundtrack sounds'          :  Displays the folder that the plugin sounds should be located (for debugging installation issues)`

## Problems?
### I cannot hear any music when I play, even with my PC volume at full!
`soundtrack sounds` will output the location that the plugin expects to find its music files. This will often help you solve your issue - make sure you have all the wav files in this location. You probably did not keep the directory structure when extracting the .zip file. If you are comfortable editting code, you could try the above suggestion and edit this location.
* The easier option is to create this folder (if it does not exist) in file manager and move the .wav files into it. If you already have other sounds in the same location, you could simply extract them from the soundtrack.zip file again.
