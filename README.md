# spearmint-msvc

[![spearmint compiling and mohaa maps](https://img.youtube.com/vi/ptBOqD5Tye0/0.jpg)](https://www.youtube.com/watch?v=ptBOqD5Tye0)

Currently works: engine, game, cgame, rend1, all you need to play nicely

Start engine project in solution with these arguments: `+set vm_cgame 0 +set vm_game 0 +set sv_pure 0`

The `vm_` stuff makes it use the .dll's

Make sure to select `Debug` / `x86`, because nothing else is configured yet.

Quick Visual Studio tutorial:
 * `F5` = `Start the "startproject"`
 * `Shift + F5` = `Kill started process`

Download Open Arena assets from here: http://openarena.ws/download.php?view.4

Find the MoHAA `.pk3` files somewhere.

`.pk3` is just renamed `.zip`, open with: https://www.7-zip.org/ (right-click -> 7-Zip -> Open archive)

MoHAA archives content (rename them to `mohaa_pak0.pk3`, because other engines use same name...):
 * `Pak0.pk3` -> anim / fffx / fonts / gfx / global / models / music / newanim / scripts / ubersound / ui
 * `Pak1.pk3` -> textures
 * `Pak2.pk3` -> textures / env
 * `Pak3.pk3` -> sound
 * `Pak4.pk3` -> sound
 * `Pak5.pk3` -> maps

Fun stuff:
 * `devmap q3dm1`
 * `devmap <tab>` --> `list of all maps`
 * `bind g noclip`
 * `g_speed 1000`

To-do:
 * add rend2 project
 * fix qvm, its crashing for some reason
 * awesome mods
 * configure Release modes and x64
