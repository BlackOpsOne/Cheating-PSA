# World at War - Stealth Cheating

## Dvars/Commands
The following commands/Dvars can be modified or used to cheat:

| Name                         |                                                         Description                                                         |
| :--------------------------- | :-------------------------------------------------------------------------------------------------------------------------: |
| `cl_noprint`                 |                                Stops printing on the screen when certain commands are used.                                 |
| `magic_chest_movable`        |                         Determines if the box can move or not. Does not exist on Nacht Der Untoten.                         |
| `ai_disableSpawn`            |                                              Stops the zombies from spawning.                                               |
| `zombie_reachin_freq`        |                               How often the zombies can reach through a window and slap you.                                |
| `zombie_taunt_freq`          |                          How often the zombies will taunt at the window after ripping a part off.                           |
| `cg_hudDamageIconTime`       |                                     How long the damage indicator is on the screen for.                                     |
| `player_reviveTriggerRadius` |                                    The radius of which you can revive another player at.                                    |
| `g_speed`                    |                                        The speed of how quickly you can move around.                                        |
| `sv_fps`                     |                       The rate that the internal server updates at, the client does not get affected.                       |
| `timescale`                  |                                   Speeds up both the server and client side of the game.                                    |
| `ai_corpseCount`             | Controls the amount of corpses that can be on the map at one time. This can be as low as `3` with the "Corpse Size" option. |
| `difficultyEasy`             |      Sets your difficulty to "Recruit", this makes you take less trap damage but makes your health regenerate slower.       |
| `difficultyHard`             | Sets your difficulty to "Hardened", this makes you take slightly more trap damage but makes your health regenerate faster.  |
| `difficultyFu`               | Sets your difficulty to "Veteran", this makes you take a lot more trap damage but makes your health regenerate way faster.  |
| `developer_script`           |            Toggles specific code that was left in by the developers for debugging, but can be abused by players.            |
| `g_disable_zombie_grab`      |                             Toggles the "stickiness" effect that the zombies in this game have.                             |
| `jump_height`                |                                          The height that the player will jump at.                                           |
| `jump_stepSize`              |                                The max you can step up to the top of a jump arc or platform.                                |

## No Printing
No printing refers to setting the Dvar `cl_noprint` to `1`, this removes any on screen messages such as god mode toggle states.

> [!CAUTION]
> This makes it impossible to know if someone is using God Mode, Demi God Mode, or No Target.

## Ingame Save States
The game has a command called `devsave` that saves the exact state of a game at any certain point, however the entity counter does not reset back to what it was.

> [!WARNING]
> This can be detected if the game is being streamed live. However if the game is played offline, combined with no printing, this is impossible to detect.

## Stealth Patching
Stealth patching is exactly what it sounds like, a patch with no indication that it is being used or that it exists, with intention of modifying the game as an advantage.

The only ways that this is done on World at War, is via Plutonium with scripts, or via the modding system that exists in the base game.

> [!CAUTION]
> Since the scripts that players put into the game are not compiled, any player can edit and remove printing of any kind that would indicate a type of patch being used.

## Dvar/Command Writing
This refers to the use of external programs to write to the command buffer to either set a certain Dvar or run a certain command.

> [!CAUTION]
> The only way to detect this is via an external program checking the game's memory.

## Fastfile Modification
Any of the base game `.ff` files in the `zone` folder can be modified with the use of fastfile extractors.

> [!CAUTION]
> If one were to modify one of the fastfiles that are loaded for Zombies, they could hide anything they wanted in it.

## GSC Injectors
These are external programs that inject GSC scripts mid game.

> [!CAUTION]
> There is no way to detect this without an external program hooking into the game.

## Custom Game Executables
The game executable itself can be modified to gain an advantage.

> [!WARNING]
> It is unknown if this detectable by simply looking at the file's size or hash, since no one ever has the same executable.

> [!CAUTION]
> The only way to detect this is via an external program checking all relevant game functions.

## Console Stealth Patching
Console can have stealth patches via GSC injector mod menus, but modifying the script to not be a mod menu but something that would provide an advantage, such as a better setup.

> [!CAUTION]
> This is impossible to detect, as console can not have a reliable anticheat.

# [Next Page: Black Ops - Obvious Cheating](../bo1/Obvious-Cheating.md)