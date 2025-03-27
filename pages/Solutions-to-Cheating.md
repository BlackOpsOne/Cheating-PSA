# The Solutions to Cheating in Zombies
With all of this information taken into account, it is recommended to do one of these things.

## Preventing Splicing
This is probably one of the longest standing cheating issues in zombies.

There are two solutions to this problem, however one will be better than the other:

### Streaming with a Unix Timestamp overlay
- In addition to just streaming, whether that is on an alternate account or an unlisted YouTube stream, you should use an overlay of some kind that displays the [Unix Timestamp](https://www.epochconverter.com) so that the community can verify that games are played when they are claimed to have been played, I have created one [here](https://github.com/BlackOpsOne/OBS-Timestamp), but there are probably others that exist. Each game still needs to be watched fully with this way.

## Live Game Monitoring
- A program that monitors when games start and end, including information like the round number and the map name, etc. That information would then be sent to lets say a public discord server via a webhook, this could work extremely well as you will always know when games are actually played. This would have to be created, but it is an idea that would work nonetheless.

## World at War
Right now, this game is waiting for Plutonium to add the checksum features to T4, then players can do the same thing they would for Plutonium on Black Ops.

## Black Ops
There are two ways to make sure games are legitimate now, and are both very public, however much like with the splicing solution above, you 

### Plutonium (Recommended)
<details>
  <summary>Click to view.</summary>
  
As of [r4811](https://plutonium.pw/docs/changelog/#r4811---t5-refactor), Plutonium for BO1 has been redone, and all issues that made the client not legit for runs in the past have been fixed.

You may be asking why would you ever use Plutonium for BO1? Because it quite literally has ways to catch cheating:

- `cg_drawChecksums` command, this will take all of the files loaded by the game and create unique hashes based on that information, this can verify if a player is patching at all, running a mod through the client, or running verified patches too, for example animated camo patches.
- Dvar/Command protection is in place now for most things, the ones that are protected require `sv_cheats` to be enabled in order to be used, and is reset once cheats is deactivated.
	- They are working on protecting more and adding an indicator for cheats being toggled.

All you have to do is have `cg_drawChecksums` set to `1` at the start of your run once, making sure the text is readable. We would suggest you have it enabled until you get a game going, then toggle it off with a bind once you have a run.

Toggle bind: `bind KEY "toggle cg_drawChecksums 0 1"`

Config path: `%LocalAppData%\Plutonium\storage\t5\players\config.cfg`
</details>

### Steam/BGamer - AntiCheat Program
<details>
  <summary>Click to view.</summary>

I myself have created an [anticheat program](https://github.com/BlackOpsOne/BO1-AntiCheat) that detects everything known and comes with future proofed detections, however requires you to show it's own file properties as part of the verification process, it is not very user friendly because of that, but it gets the job done at the end of day.

</details>

## Black Ops II
There is a very simple solution for this game:
- Use the latest version of Plutonium, it has the feature for checksums which is important.
- Use a patch that forces the flashing of the patch checksums or toggling of `cg_drawChecksums`.
- Any patches that are unknown should be an instant game dismissal, as any unknown patch can do anything (as an example, survival map trade luck patches are out there, so this is important), so only use the patch that is trusted.

## Black Ops III
A custom [BOIII](https://github.com/Ezz-lol/boiii-free) client needs to be created, with probably the same features that Plutonium has for Black Ops with the checksums and Dvar/Command protection.

# What does the community do with this info?
The ways to verify games properly has been laid out for you, now its just up to the communities of each game to the necessary steps to make the solutions a reality, or even improve off of them.