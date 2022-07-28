Edit:------------------------------------------------
Edited "IGCSInjector " for Northstar Compatilbility

From:
[InjectionData]
Process=Titanfall2.exe
Dll=Titanfall2CameraTools.dll

To:
[InjectionData]
Process=NorthstarLauncher.exe
Dll=Titanfall2CameraTools.dll
------------------------------------------------------

Injectable camera for Titanfall 2 v1.0+
============================
Camera version: 1.0.3
Camera credits: Otis_Inf.
Powered by Injectable Generic Camera System by Otis_Inf.
https://github.com/FransBouma/InjectableGenericCameraSystem
----------------------------------------------------------------

Ctrl-Ins                              : Show / Hide Camera tools main window
Ctrl + Mouse wheel                    : Resize font
Del                                   : Toggle first/third person (not when camera is active)
Ins                                   : Enable/Disable camera
Home                                  : Lock/unlock camera movement
ALT + rotate/move                     : Faster rotate / move
Right-CTRL + rotate/move              : Slower rotate / move
Controller Y-button + l/r-stick       : Faster rotate / move
Controller X-button + l/r-stick       : Slower rotate / move
Arrow up/down or mouse or r-stick     : Rotate camera up/down
Arrow left/right or mouse or r-stick  : Rotate camera left/right
Numpad 8/Numpad 5 or l-stick          : Move camera forward/backward
Numpad 4/Numpad 6 or l-stick          : Move camera left / right
Numpad 7/Numpad 9 or l/r-trigger      : Move camera up / down
Numpad 1/Numpad 3 or d-pad left/right : Tilt camera left / right
Numpad +/- or d-pad up/down           : Increase / decrease FoV
Numpad * or controller B-button       : Reset FoV
Numpad .                              : Block input to game for camera control device.
Numpad 0                              : Toggle game pause

Changes
===========
v1.0.3: 
- Yet another write found which is only used in some cutscenes (hence I missed it). This one is now blocked too and the camera should 
now work in *all* cutscenes.

v1.0.2: 
- Added DoF controls to the settings
- Added a button to open the command console, so it's not opened if not needed.
- Added 6 more write blocks of code writing to the camera coords/angles. These didn't seem necessary as they wrote the same values back but in 
some occasions they did appear to cause problems
- Added a more stable block for a write block so it won't crash the game anymore. 

v1.0.1: 	
- Added in-game command console which opens when the camera menu is opened. It allows you to pass commands to the game, it doesn't 
enlist output from commands, just allows you to execute commands. Not a lot of them work, mind you. 
- Added first/third person switch using the DEL key so no need for custom config files anymore. 

Important
===========
- This is the last public binary release of a camera I've made. All potentially future cameras will be released as
source only. It simply takes too much time to polish them up to release quality. I'll hand out binaries to 
friends if necessary.
- Even though I took a lot of care to make this a stable release, there are situations, especially in cutscenes where the game will crash when you
enable the camera. I don't know how to fix it, so you can ask, but I don't have the answer. 
- USE IN SINGLE PLAYER ONLY. NO EXCEPTIONS / EXCUSES
- Inject the camera AFTER you've loaded a level. It relies on the engine object which isn't known at startup.

Support
===========
There's no support. If the camera breaks while I'm using it, it'll be updated, otherwise you're out of luck and
you have to fix it yourself (the source is right here on github!). Please don't ask questions like how to use the
camera, how to build the source etc. as I won't answer them if I don't know you. 

How to use
===========
Run the game as Administrator. This is very important. Then start IGCSInjector.exe. It will show a dialog that things are injected fine, 
or if an error occurred, it will tell you that too. 
You should get a notification in the top left corner of the game window. Open the in-game main window with settings, help and console
using Ctrl-Ins. Start the injector slightly later than the game so hooking into the XInput (for controller blocking) is picked up. 

HUD Toggle
===========
Use the hud toggle by The Janitor:
http://www.moddb.com/games/titanfall-2/downloads/toggle-hud5

"Your in-game main window is too tiny on my 4K screen!"
=======================================================
Click it, then hold Ctrl while using your mouse window to zoom the text, then resize it. In case you're wondering, yes that's the
same trick you can use with Reshade 3. This setting isn't preserved however, so you have to do that every time you start the game. 

"After I switched to a high resolution and moved the window, going back to a low resolution doesn't show the in-game window"
=============================================================================================================================
It's still there, but outside the visible area on the screen. Either go back to the high resolution, open the in-game window, 
and move it to the top left corner, or remove the IGCS_Overlay.ini file in the game's root folder and restart the game. 

Camera control device
========================
In the camera menu, you can specify what to use for controlling the camera: controller, keyboard+mouse, or both. The device you pick is
blocked from giving input to the game, if you press 'Numpad .'. You can also specify if you want to have the device active when the menu is 
showing. If you've chosen keyboard+mouse for camera control, and you still want to use that feature, you of course don't want to move 
the camera when moving the mouse for the menu. To avoid that, press 'Home' key to lock the camera so you can move the mouse. Pressing 'Home' 
again will unlock the camera. 

Have fun and create beautiful shots, m'kay? 

Cheers!

Otis_Inf