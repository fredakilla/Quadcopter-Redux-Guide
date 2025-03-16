# Guide for Quadcopter-Redux

Here is a practical guide to use the FPV Quadcopter-Redux drone simulator on GTA V.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Quadcopter-Redux.jpg)

## Installation

- Of course, you need to have the GTA V game (no matter where it comes from: steam, epic store or others...)   
- ScriptHookV : A library that allows to interface with GTA to create mods.   
- ScriptHookVDotNet : An extension of the previous library to use the .NET technology   
- Quadcopter-Redux : The mod that contains the simulator.   


Install each library independently:       
Here are the links to the files to install (take the latest versions for each) :   
[http://www.dev-c.com/gtav/scripthookv/](https://www.dev-c.com/gtav/scripthookv/)   
[https://github.com/crosire/scripthookvdotnet/releases](https://github.com/scripthookvdotnet/scripthookvdotnet-nightly/releases/tag/v3.7.0-nightly.20)      
[https://www.gta5-mods.com/scripts/quadcopter-redux  ](https://fr.gta5-mods.com/scripts/quadcopter-redux)    

You just have to unzip all these files in the GTA game installation directory, and that's it.

Make sure the files are in the right place.   
For the ScriptHookV zip archive, it is the content of the bin folder that you have to put in the root of the game.   
Here is for example what you should normally find in the root of the GTA game:   

```
E:\SteamLibrary\steamapps\common\Grand Theft Auto V\  

// ScriptHookV files :
dinput8.dll
NativeTrainer.asi
ScriptHookV.dll

// ScriptHookVDotNet files :
ScriptHookVDotNet.asi
ScriptHookVDotNet.ini
ScriptHookVDotNet2.dll
ScriptHookVDotNet2.xml
ScriptHookVDotNet3.dll
ScriptHookVDotNet3.xml

// Quadcopter-Redux files :
soft_oal.dll
scripts\Quadcopter\img\
scripts\Quadcopter\sounds\
scripts\Quadcopter\GTA5-Quadcopter.dll
scripts\Quadcopter\Changelog.txt
```

And if you press F4 in game you should acces to the ScriptHookV menu, this means that it is correctly installed.

```diff
! Possible issue
Nothing when pressing 'G' ?
If you see the "quadcopter-redux loaded" message in the upper-left corner when entering the game, everything is ok.
But on some systems there is a permission access issue because the GTA folder can be read-only and ScriptHookV and
Quadcopter-Redux at startup try to write their settings or log files if they doesn't exists yet in this folder.   
Try going into the security of the GTA folder and give it write access.

(The Steam version should fix this but I know that this problem can be encountered on the versions coming from the 
Rockstar Games Launcher, I have no feedback yet on the Epic store versions)
```

**Important note:** The use of mods for GTA V is not officially recognized nor encouraged by the publisher Rockstar, however this practice is tolerated as long as it remains for offline mode content (so for the story in single player mode). If you plan to play GTA online, it is recommended to remove the mods anyway ScriptHookV will prevent you from playing in online mode to avoid being banned and cheating.

## Running the simulator
Run GTA in story mode, the simulator mod will be automatically detected. Once in game you can use the following keys:

- G : To switch to drone/player mode
- H : To stop flying and teleport player to the drone position
- F10 : to open the simulator menu (only when you are in drone mode)
- PageUp / PageDown : camera tilt
- R : To reset the drone, if you are stuck
- C : to change the camera view
- F : to switch between acro or angle flight mode
- X : Abort mission (for active events)
- B : Restart last mission (for active events)


## First time installation
If you install for the very first time GTA V and you launch the game, you will have to complete the intro which lasts about fifteen minutes and which plunges you in the universe of the game but on a small map to teach you how to play. Once you pass this intro you will have total access to the huge GTA map and you will be able to use the simu without any constraint.

But don't worry, you don't have to go through this intro at all or even do the GTA missions if you want to use this game exclusively in FPV drone simulator mode with Quadcopter-Redux.

The easiest way to do this is to download a savegame that completes the game 100%.

You can download a savegame from this page:   
https://fr.gta5-mods.com/misc/100-game-save-for-1-7

Install the savegame on your PC at the location indicated on the description page and restart the game, you will be able to use Quadcopter-Redux directly without going through the intro and you will be propelled to the end of the game with all missions already completed.

## Controller configuration
It is highly recommended to use a real FPV drone radio-controller to pilot with precision the drone in the simulator and find the same sensations and precision as in real life.

If you don't have a radio, it's possible to use a gamepad like xbox360 to learn or test this mod but it's really not recommended because you risk to take bad reflexes with this kind of controller which is not precise enough nor adapted to fly a drone, especially for the throttle stick which spring is disabled on a real radio.

Most radio controllers should be automatically detected.

here is a list of radios known to work with this mod:

- TBS tango 2
- DJI FPV controller 2 (the one of the avata and the DJI FPV)
- BetaFPV LiteRadio 2 SE
- Radiomaster TX12 / TX16

For the configuration, open the menu of the drone. Go to the submenu 'Gamepad'.

Activate 'direct input' if you have a radio controller otherwise deactivate it to use a gamepad like xbox360.

Change the value of the sticks in order to affect correctly the throttle, pitch, yaw and roll. You can use the gauges and the text indicator to detect the index of the stick you are touching.

And do the same if you want to bind buttons, like for example the engine arming, the unstuck button, or the fire button...

It's also recommended to run a stick calibration, press calibration menu item and move you stick in all directions up to the limits, press calibration menu item to end process.  

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Controller.jpg)


## Rates Configuration
The 'controller' menu allows you to define your rates to obtain the desired rotation speed. The supported modes are Actual, Betaflight, Kiss and Raceflight.

It is possible to use up to 3 slots to save different rate configurations.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Rates2.jpg)

## Drone configuration
Go to the 'Drone Presets' menu to configure your drone.

You can create many different presets to represent different types of drone.   
Drone presets are saved as .txt files in the scripts\Quadcopter\drone_presets directory.   

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/DronePreset.jpg)


## Additional content
The modding community around GTA is huge and many mods have been made. You can enrich your experience with this simulator even more by adding additional mods.

Here is a small list of mods that I recommend:   

Native Trainer (provided with ScriptHookV) : allows you to do a lot of things (teleportation, change weather, time, etc...)   
[Menyoo](https://www.gta5-mods.com/scripts/menyoo-pc-sp) : Multi purpose trainer and map editor to create your own courses or race tracks.   
[Forests of San Andreas](https://www.gta5-mods.com/maps/forests-of-san-andreas-revised) : Greatly improves the density and variety of trees for beautiful forest walks.    
[GTA V Remastered: Enhanced](https://www.gta5-mods.com/maps/gta-v-remastered-enhanced) : Enhances some parts of the map by adding more detail.  
[QuantV](https://www.gtainside.com/en/gta5/mods/119996-quantv-2-1-4) : Redesign and overall improvement of GTA graphics, lighting and weather effects.   
