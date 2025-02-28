# Black Ops - Stealth Cheating

## Dvars/Commands
The following commands/Dvars can be modified or used to cheat:

| Name                            |                                                         Description                                                         | Default Value |
| :------------------------------ | :-------------------------------------------------------------------------------------------------------------------------: | :-----------: |
| `cl_noprint`                    |                                Stops printing on the screen when certain commands are used.                                 |      `0`      |
| `sv_cheats`                     |                  Toggles the use of cheats like god mode. On solo this is set to `1` by default it seems.                   |      `0`      |
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
| `jump_height`                   |                                          The height that the player will jump at.                                           |     `39`      |
| `jump_stepSize`                 |                                The max you can step up to the top of a jump arc or platform.                                |     `18`      |
| `cl_dtpHoldTime`                |                 The amount of milliseconds you must hold the `Change Stance` key in order to dolphin dive.                  |     `200`     |
| `dtp_exhaustion_window`         |                               The amount of milliseconds you must wait to dolphin dive again.                               |    `1500`     |
| `dtp_fall_damage_max_height`    |                               The max height you must dolphin dive from to take fall damage.                                |     `200`     |
| `dtp_fall_damage_min_height`    |             The min height you must dolphin dive from to take fall damage, PHD Flopper will also activate here.             |     `65`      |
| `dtp_min_speed`                 |                        The minimum speed you must be running at to start or sustain a dolphin dive.                         |    `3.16`     |
| `dtp_new_trajectory`            |                                     Toggles the new dolphin diving trajectory equation.                                     |      `1`      |
| `dtp_new_trajectory_multiplier` |                                         The multiplier for the new dive trajectory.                                         |      `2`      |
| `dtp_post_move_pause`           |                            The amount of milliseconds that you can not move for after flopping.                             |     `100`     |
| `dtp_startup_delay`             |                         Determines how long the player has to sprint for in order to dolphin dive.                          |     `250`     |

## No Printing
No printing refers to setting the dvar `cl_noprint` to `1`, this removes any on screen messages such as god mode toggle states.

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
> This DLL can be injected at any point in the game, and the custom `.ff` file can be swapped out and back in at any point.
>
> This makes the showing of your files completely useless, the point of that rule was to prevent launching from a third party launcher containing this method.
>
> The only way to detect this is via an external program checking the game's memory and loaded DLL files.

## GSC Injectors
These are external programs that inject GSC scripts mid game.

> [!CAUTION]
> There is no way to detect this without an external program hooking into the game.

## Dvar/Command Writing
This refers to the use of external programs to write to the command buffer, to either set a certain dvar or run a certain command.

> [!CAUTION]
> The only way to detect this is via an external program checking the game's memory.

## Zolfernos
Zolfernos is a trainer for Black Ops Zombies, it allows you to write to memory on a multitude of different levels.

> [!CAUTION]
> This is undetectable and changes multiple aspects of the game.

## Custom BGamer Launchers
Launching the game from certain BGamer launchers that have been modified by players is known to inject the Stealth Patch DLL mentioned [here](#stealth-patching---dll-injection).

> [!WARNING]
> This can be detected but there are ways to spoof the date modified. The estimated file size can remain the same as well as it doesn't take much to modify the launcher.
>
> You would need to show the file properties to know the exact amount of bytes.

## Custom Game Executables
The game executable itself can be modified to gain an advantage.

> [!CAUTION]
> This can lead to a multitude of changes that are not possible via a patch.
> The only way to detect this is via an external program checking all relevant game functions. Checking hashes will not work due to how Steam downloads files, the game executable is never the same for some reason.

## Console Stealth Patching
Console can have stealth patches via GSC injector mod menus, but modifying the script to not be a mod menu but something that would provide an advantage, such as a better setup.

> [!CAUTION]
> This is impossible to detect, as console can not have a reliable anticheat.

## Shader Warming
Shader warming can be used to splice a raw session or run very easily, as it is a completely static screen.

> [!TIP]
> There is a very simple solution to this, ban Shader Warming.

## Patch Insertion Programs
Players have created programs to place both modified and vanilla fastfiles in the `zone` folder.

> [!WARNING]
> This does appear to place vanilla files into the game if a player selects it. However, I must reiterate that vanilla fastfiles can be modified with zero indication that they've been modified.
>
> This is a semi private tool, we have no idea whats in the fastfiles from it. Any tool that does this can put any kind of patch in the game.

# [Next Page: Black Ops II - Cheating](../bo2/Cheating.md)