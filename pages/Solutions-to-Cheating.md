# The Solutions to Cheating in Zombies

## Preventing Splicing
This is probably one of the longest standing cheating issues in zombies.

The only real way to prove that a game is not spliced, is likely going to be each game being verified with an anticheat or some kind of program that constantly monitors a game, with lots of information about the game such as the current round number, when it started/ended, etc.

That information should be saved publicly in some way so that the community can go back and tell if a certain game was fully played or not based on the game data collected.

## World at War
Right now this game needs to wait for Plutonium to add the patch checksums feature, then a patch can be created to force the flashing of it.

## Black Ops
What you as a player can do:
- Showing that you launch the game from `BlackOps.exe` to prevent any runtime injections.
  - Do NOT launch from the BGamer Launcher or any third party launcher, ensure you start from the game executable.
    - If using BGamer, simply start hostmode and then open the game executable.
    - The reason for this is the fact that there are BGamer launchers (and batch scripts) that force the game to load stealth patches, they are also actively being passed around in certain parts of the community.
- Showing the the entire `zone` folder and all of its subdirectories.
  - Make sure any extra files are removed from these folders, as the extra files are deemed as stealth patches.
- Showing that hidden files are enabled.
  - This proves that you do not have any extra files.

At the end of the day, [BO1-AntiCheat](https://github.com/BlackOpsOne/BO1-AntiCheat) is the most secure solution, it picks up on everything known and comes with future proofed detections.

## Black Ops II
What you as a player can do:
- Use a patch that forces the flashing of the patch checksums.
- Any patches that are unknown should be an instant game dismissal, as it can do anything, so only use the patch that is trusted.
- The latest version of Plutonium, as they do have an anticheat in the client that should catch external programs.

## Black Ops III
The only way to prevent proper cheating on this game is an anticheat, this can be done with a custom [BOIII](https://github.com/Ezz-lol/boiii-free) client, however needs to basically monitor the entire game.

# What will eventually have to happen
Sometime in the future, the only solution that will work is an actively updated anticheat for each game that is specifically designed to catch everything that is known and also try to prevent other things that people may try to do.

Anything in between now and then are only temporary fixes to the problem.