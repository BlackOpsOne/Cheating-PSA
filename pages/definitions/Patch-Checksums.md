# Definitions - Patch Checksums

On Plutonium r4516 and above, there is a feature that will flash the unique checksums of all the scripts/patches loaded. You can make these flash by setting the Dvar `cg_flashScriptHashes` to `1`, this will flash them on the top left of the screen once the initial black screen fades away.

The unique checksum of a patch will change if it is changed in any way. These can be used to verify if a community verified patch has been modified or not.

Also, there is a new dvar called `cg_drawChecksums`, once set to `1`, this will display checksums of your current game, this takes everything loaded into account when calculated. These are unique and will change upon different patches/scripts being loaded.

# [Next Page: World at War - Obvious Cheating](../waw/Obvious-Cheating.md)