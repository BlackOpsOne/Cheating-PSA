# Black Ops II - Cheating
Since this game has a small amount of obvious methods, which are able to be made into stealth methods anyways, I have decided to combine them into one place.

## Dvars/Commands
The following commands/Dvars can be modified or used to cheat:

| Name                            |                                                         Description                                                         | Default Value |
| :------------------------------ | :-------------------------------------------------------------------------------------------------------------------------: | :-----------: |
| `con_gameMsgWindow0MsgTime`     |                        The amount of time that god mode and other printed messages will appear for.                         |      `5`      |
| `sv_cheats`                     |                                          Toggles the use of cheats like god mode.                                           |      `1`      |
| `magic_chest_movable`           |                       Determines if the box can move or not. This is set to `0` on Nacht Der Untoten.                       |      `1`      |
| `ai_disableSpawn`               |                                              Stops the zombies from spawning.                                               |      `0`      |
| `zombie_reachin_freq`           |                               How often the zombies can reach through a window and slap you.                                |     `50`      |
| `zombie_taunt_freq`             |                          How often the zombies will taunt at the window after ripping a part off.                           |      `5`      |
| `player_reviveTriggerRadius`    |                                    The radius of which you can revive another player at.                                    |     `64`      |
| `g_speed`                       |                                        The speed of how quickly you can move around.                                        |     `190`     |
| `timescale`                     |                                   Speeds up both the server and client side of the game.                                    |      `1`      |
| `ai_corpseCount`                | Controls the amount of corpses that can be on the map at one time. This can be as low as `3` with the "Corpse Size" option. |      `5`      |
| `developer_script`              |            Toggles specific code that was left in by the developers for debugging, but can be abused by players.            |      `0`      |
| `scr_force_weapon`              |             Sets the weapon you want out of the box, this is only usable when `developer_script` is set to `1`.             |      ` `      |
| `g_banzai_player_fov_buffer`    |      Determines the fraction of a player's FOV that the game uses to determine if a zombie should despawn by distance.      |     `0.2`     |
| `jump_height`                   |                                          The height that the player will jump at.                                           |     `39`      |
| `jump_stepSize`                 |                                The max you can step up to the top of a jump arc or platform.                                |     `18`      |
| `dtp_exhaustion_window`         |                               The amount of milliseconds you must wait to dolphin dive again.                               |    `1500`     |
| `dtp_fall_damage_max_height`    |                               The max height you must dolphin dive from to take fall damage.                                |     `200`     |
| `dtp_fall_damage_min_height`    |             The min height you must dolphin dive from to take fall damage, PHD Flopper will also activate here.             |     `100`     |
| `dtp_min_speed`                 |                        The minimum speed you must be running at to start or sustain a dolphin dive.                         |    `3.16`     |
| `dtp_new_trajectory`            |                                     Toggles the new dolphin diving trajectory equation.                                     |      `1`      |
| `dtp_new_trajectory_multiplier` |                                         The multiplier for the new dive trajectory.                                         |      `2`      |
| `dtp_post_move_pause`           |                            The amount of milliseconds that you can not move for after flopping.                             |     `100`     |
| `dtp_startup_delay`             |                         Determines how long the player has to sprint for in order to dolphin dive.                          |     `250`     |

## No Printing
No printing refers to setting the dvar `con_gameMsgWindow0MsgTime` to `0`, this removes any on screen messages such as god mode toggle states.

> [!TIP]
> The state of this is not retained in demos, likely because they are client based Dvars and not server based.

> [!CAUTION]
> This makes it impossible to know if someone is using God Mode.

## Modification of Community Patches
The community has created patches that have legitimate use cases such as automatic timers, however there are recompiled versions of them floating around that contain ways to cheat, such as increased box luck on survival maps.

> [!TIP]
> This is detectable via [patch checksums](../definitions/Patch-Checksums.md).

> [!CAUTION]
> Unofficial versions of community patches can include more than just what the base patch has, such as modified luck on many aspects of the game.

## Custom Patches/Scripts
A player can create their own scripts and put them into the scripts folder in order to modify how the base game works.

> [!CAUTION]
> On versions of Black Ops II that do not contain the checksums feature, this is undetectable.

## Dvar/Command Writing
This refers to the use of external programs to write to the command buffer, to either set a certain dvar or run a certain command.

> [!TIP]
> Some patches will detect when certain Dvars are changed, such as `sv_cheats`.

> [!CAUTION]
> The god mode state can be activated via a script.
> 
> The only way to detect this is via an external program checking the game's memory.

## Custom Game Executables
The game executable itself can be modified to gain an advantage.

> [!TIP]
> Luckily, the exact same game executable is provided by Plutonium every time. Redacted also uses the same executables, so this is detectable by simply checking the hash.

> [!CAUTION]
> This can lead to a multitude of changes that are not possible via a patch.

## Console Stealth Patching
Console can have stealth patches via GSC injector mod menus, but modifying the script to not be a mod menu but something that would provide an advantage, such as a better setup.

> [!CAUTION]
> This is impossible to detect, as console can not have a reliable anticheat.

# [Next Page: Black Ops III - Obvious Cheating](../bo3/Obvious-Cheating.md)