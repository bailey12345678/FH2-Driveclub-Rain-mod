# FH2-Driveclub-Rain-mod
Driveclub-style windscreen rain for Forza Horizon 2 on Azimuth (PC): water on the glass, cleared by the game's own wipers.

FH2 Driveclub rain  -  V 1.0.1
==============================

Driveclub-style rain on the windscreen for Forza Horizon 2 (Azimuth, PC). Water collects and runs on the glass, the game's
own wipers push it away where they touch it, and it gets wetter when FH2's weather turns to a storm.


WHAT YOU NEED
-------------
- Forza Horizon 2 running on Azimuth 1.0.4 (tested with that version).
- Nothing else. Everything else this mod needs is in this zip.


INSTALL (about a minute)
------------------------
1. Close the game.
2. Open the folder that contains azimuth.exe.
3. Extract this zip straight into that folder (choose "Extract here" / "Extract All" and point it at the azimuth.exe folder).
   If Windows asks whether to replace files, say Yes.
4. Start the game. That's it.

After extracting, your azimuth.exe folder should contain these (alongside everything that was already there):

    azimuth.exe                          (yours, untouched)
    d3dcompiler_47.dll                   FH2 Mod Platform - loads the mods in fh2-mods
    mods\FH2 Mod Platform\               starts the FH2 Mod Platform on Azimuth 1.0.4
    fh2-mods\FH2 Driveclub rain.dll      the mod
    FH2 Driveclub rain\                  its settings and per-car data

To check it's running: in the game's pause menu, open the MODS page. You should see "FH2 Driveclub rain   V 1.0.1".


HOW TO USE IT
-------------
Get in a car in cockpit view and wait for rain (or set rain from a weather mod if you have one). The windscreen water
switches on by itself a second or two after you get in.

Keys (keyboard):
  F5   one wipe
  F6   wiper mode: AUTO > OFF > INTERMITTENT > NORMAL > FAST > AUTO
       AUTO is the game's own wiper rhythm.

To change the keys or switch things off, open  FH2 Driveclub rain\FH2 Driveclub rain.ini  in Notepad:
  SingleWipeKey=116   key for one wipe (116 = F5). Uses Windows key codes.
  WiperModeKey=117    key for the wiper mode (117 = F6).
  Enabled=0           turns the whole mod off (the game's normal rain comes back).
Save the file and restart the game.


GOOD TO KNOW
------------
- 322 cars are supported with their own wiper layout. A car without one (a few rare cars, and cars with three wipers such
  as the E-Type) simply keeps the game's normal windscreen rain.
- Cars an event hands you (not from your garage) are recognised automatically by their wipers.
- Storm is heavier than light rain mainly when parked or slow. At speed the glass is already as full as the water
  simulation allows, as in Driveclub itself.
- If your frame rate stays below 40 for five seconds, the mod pauses its water and the normal rain comes back, so the game
  stays playable.


ALREADY HAVE OTHER FH2 MODS?
----------------------------
If you already use mods that live in an  fh2-mods  folder (they need the same FH2 Mod Platform), they keep working.
Replacing d3dcompiler_47.dll with the one in this zip is fine; it is the same kind of loader.


UNINSTALL
---------
Delete  fh2-mods\FH2 Driveclub rain.dll  and the  FH2 Driveclub rain  folder.
If no other mod in fh2-mods needs it, you can also delete  d3dcompiler_47.dll  and  mods\FH2 Mod Platform.


SOMETHING NOT WORKING?
----------------------
- Not on the MODS page: check that d3dcompiler_47.dll sits right next to azimuth.exe (not in a sub-folder), and that
  "mods\FH2 Mod Platform" is inside the azimuth.exe folder.
- Normal rain instead of Driveclub water: look in  fh2-mods\platform.log  for lines starting with [FH2 Driveclub rain].
  "no reference" means that car isn't supported (it keeps normal rain).


CHANGES
-------
V 1.0.1  Fast travel no longer gives your car another car's wipers: only the cockpit you are sitting in is ever recognised.
V 1.0    First release.
