# Black Ops: Stealth Cheating

## Dvars/Commands
The following commands/Dvars can be modified or used to cheat:

| Name                            |                                                         Description                                                         | Default Value |
| :------------------------------ | :-------------------------------------------------------------------------------------------------------------------------: | :-----------: |
| `cl_noprint`                    |                                Stops printing on the screen when certain commands are used.                                 |      `0`      |
| `magic_chest_movable`           |                       Determines if the box can move or not. This is set to `0` on Nacht Der Untoten.                       |      `1`      |
| `ai_disableSpawn`               |                                              Stops the zombies from spawning.                                               |      `0`      |
| `zombie_reachin_freq`           |                               How often the zombies can reach through a window and slap you.                                |     `50`      |
| `zombie_taunt_freq`             |                          How often the zombies will taunt at the window after ripping a part off.                           |      `5`      |
| `cg_hudDamageIconTime`          |                                     How long the damage indicator is on the screen for.                                     |    `2000`     |
| `player_reviveTriggerRadius`    |                                    The radius of which you can revive another player at.                                    |     `64`      |
| `g_speed`                       |                                        The speed of how quickly you can move around.                                        |     `190`     |
| `sv_fps`                        |                       The rate that the internal server updates at, the client does not get affected.                       |     `20`      |
| `timescale`                     |                                   Speeds up both the server and client side of the game.                                    |      `1`      |
| `ai_corpseCount`                | Controls the amount of corpses that can be on the map at one time. This can be as low as `3` with the "Corpse Size" option. |      `5`      |
| `difficultyEasy`                |      Sets your difficulty to "Recruit", this makes you take less trap damage but makes your health regenerate slower.       |
| `difficultyHard`                | Sets your difficulty to "Hardened", this makes you take slightly more trap damage but makes your health regenerate faster.  |
| `difficultyFu`                  | Sets your difficulty to "Veteran", this makes you take a lot more trap damage but makes your health regenerate way faster.  |
| `developer_script`              |            Toggles specific code that was left in by the developers for debugging, but can be abused by players.            |      `0`      |
| `scr_force_weapon`              |             Sets the weapon you want out of the box, this is only usable when `developer_script` is set to `1`.             |      ` `      |
| `scr_force_quantum_bomb_result` |        Sets the result you want out of the QEDs on Moon, this is only usable when `developer_script` is set to `1`.         |      ` `      |
| `g_banzai_player_fov_buffer`    |      Determines the fraction of a player's FOV that the game uses to determine if a zombie should despawn by distance.      |     `0.2`     |

## No Printing
No printing refers to setting the dvar `cl_noprint` to `1`, this removes any printing at the top left from certain commands in Call of Duty.

> [!CAUTION]
> This makes it impossible to know if someone is using God Mode, Demi God Mode, or No Target.

## Stealth Patching - Game Mod
This refers to the use of Game Mod, and using a custom `.ff` file in the form of a map patch, but with `_override.ff` at the end of the file instead of just `_patch.ff`.

> [!TIP]
> This can be detected by watching how a player launches the game. It must be via the game's executable file.

> [!WARNING]
> This is not a perfect method of cheating due to how much gets changed with Game Mod. However, since the project is fully open source, a custom version of Game Mod can be built to remove the things that make it obvious that someone is using it.

## Stealth Patching - DLL Injection
This refers to the end of the last point of a modified Game Mod DLL with everything except the map override fastfile loading removed.

> [!CAUTION]
> This DLL can be injected at any point in the game, and the custom `.ff` file can be swapped out and back in at any point too.
>
> In other words, someone can be legit one game, but cheating the next, and you would never know.
>
> This makes the showing of your files completely useless, the point of that rule was to prevent launching from a script containing this method.

## GSC Injectors
These are external programs that inject GSC scripts mid game.

> [!CAUTION]
> There is no way to detect this without an external program hooking into the game.

## Dvar/Command Writing
This refers to the use of external programs to write to the command buffer, to either set a certain dvar or run a certain command.

> [!CAUTION]
> The only way to detect this is via an external program checking the game's memory.

## Custom BGamer Launchers
Launching the game from certain BGamer launchers will inject the Stealth Patch DLL method mentioned [here](#stealth-patching---dll-injection).

> [!TIP]
> This can be detected by watching how a player launches the game as the file estimated file size of the launcher will be shown. They must show themselves launching via the game's executable file regardless.

## Custom Game Executables
The game executable itself can be modified to gain an advantage.

> [!WARNING]
> It is unknown if this detectable by simply looking at the file's size or hash, since no one ever has the same executable.

> [!CAUTION]
> The only way to detect this is via an external program checking all relevant game functions.

## Console Stealth Patching
Console can have stealth patches via GSC injector mod menus, but modifying the script to not be a mod menu but something that would provide an advantage, such as a better setup.

> [!CAUTION]
> This is impossible to detect, console is the weak link.

# [Next Page: The Solution to Cheating](../Solution-to-Cheating.md)
