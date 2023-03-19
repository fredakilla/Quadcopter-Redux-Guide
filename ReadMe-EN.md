# Guide for Quadcopter-Redux

Here is a practical guide to use the FPV Quadcopter-Redux drone simulator on GTA V.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Quadcopter-Redux.jpg)

## Installation

- Of course, you need to have the GTA V game (no matter where it comes from: steam, epic store or others...)   
- ScriptHookV : A library that allows to interface with GTA to create mods.   
- ScriptHookVDotNet : An extension of the previous library to use the .NET technology   
- Quadcopter-Redux : The mod that contains the simulator.   
- 
Here are the links to the files to install (take the latest versions for each) :   
http://www.dev-c.com/gtav/scripthookv/   
https://github.com/crosire/scripthookvdotnet/releases   
https://www.gta5-mods.com/scripts/quadcopter-redux  

You just have to unzip all these files in the GTA game installation directory, and that's it.

**Important note:** The use of mods for GTA V is not officially recognized nor encouraged by the publisher Rockstar, however this practice is tolerated as long as it remains for offline mode content (so for the story in single player mode). If you plan to play GTA online, it is recommended to remove the mods to avoid being banned from the online mode and avoid cheating.

## Launching the simulator
Launch GTA in story mode, the simu will be automatically detected. Once in game you can use the following keys:

- G : To switch to drone mode
- H : To stop flying and return to the character
- F9 : to open the simulator menu (when you are in drone mode)
- PageUp / PageDown : for the tilt camera
- R : To reset the drone if you are stuck
- C : to change the camera
- F : to switch between acro or angle flight mode
- X : Abort mission
- B : Restart last mission


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

Here is the list of radios with which I could test the game:

- TBS tango 2
- DJI FPV controller 2 (the one of the avata and the DJI FPV)
- BetaFPV LiteRadio 2 SE
- Radiomaster TX12

For the configuration, open the menu of the drone. Go to the submenu 'Gamepad'.

Activate 'direct input' if you have a radio controller otherwise deactivate it to use a gamepad like xbox360.

Change the value of the sticks in order to affect correctly the throttle, pitch, yaw and roll. You can use the gauges to detect the index of the stick you are touching.

And do the same if you want to bind buttons, like for example the engine arming, the unstuck button, or the fire button...

You can also adjust the precision of the sticks from this menu or add deadband.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Gamepad.jpg)

## Rates Configuration
The 'controller' menu allows you to define your rates to obtain the desired rotation speed. The supported modes are Actual, Betaflight, Kiss and Raceflight.

It is possible to use up to 3 slots to save different rate configurations.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Rates.jpg)

## Drone configuration
Go to the 'Physx' menu to adjust the flight behavior.

You can define several slots to save different configurations to represent different types of drone.

To configure your drone, you can proceed as follows:

Start by defining the size of the propellers (in inches)
Then the weight of the drone (in Kg)
Then adjust the thrust force of the motors by testing the acceleration and the top speed to try to find the same feeling as with your real drone.
Then adjust the other factors such as gravity, drag coef or air resistance, as well as linear damping to the feeling to adjust your sensations.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Physx.jpg)

## Additional content
The modding community around GTA is huge and many mods have been made. You can enrich your experience with this simulator even more by adding additional mods.

Here is a small list of mods that I recommend:   

Native Trainer (provided with ScriptHookV) : allows you to do a lot of things (teleportation, change weather, time, etc...)   
[Map Editor](https://www.gta5-mods.com/scripts/map-editor) : A map editor to create your own courses or race tracks.   
[Forests of San Andreas](https://www.gta5-mods.com/maps/forests-of-san-andreas-revised) : Greatly improves the density and variety of trees for beautiful forest walks.    
[GTA V Remastered: Enhanced](https://www.gta5-mods.com/maps/gta-v-remastered-enhanced) : Enhances some parts of the map by adding more detail.  
