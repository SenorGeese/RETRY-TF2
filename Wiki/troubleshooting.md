---
description: Troubleshooting for Installing Custom Skins.
---

# Troubleshooting

### General Troubleshooting

<details>

<summary>Northstar Skin mods</summary>

If the skin is reactive, animated or does something special outside of just basic textures, it's probably installed as a Northstar mod. Check the skin to see if it says to be installed as a mod.

This includes the custom models such as the Cat ears. They are installed as Northstar mods.

You don't need the skin tool for these Northstar mods.

So just disable the mod.

</details>

### DDS (skintool method)

<details>

<summary>TF2 or  Northstar is running. Close it.</summary>

Pretty simple. We cannot overwrite data in the starpak if it's busy being used by the game.&#x20;

Close out of the game.

</details>

<details>

<summary>Integrated Graphics</summary>

You just can't use custom skins, as it requires Texture Streaming.

This is likely because you are using a laptop, but not all laptops are the same. Some laptops will have dedicated GPU's which allow for Texture Streaming.

</details>

<details>

<summary>TF2 Video Settings</summary>

* Open Titanfall 2.
* Navigate to Video settings.
* Check that your 'Texture Filtering' is set to at least 'Anisotropic 8x' (preferably 'Anisotropic 16X').
* Check that your 'Texture Streaming Budget' is sufficient.

</details>

<details>

<summary>NVIDIA Control Panel Settings</summary>

\*If you have a Nvidia graphics card.\*

* Open 'NVIDIA Control Panel'
* Navigate to 3D Settings**>>**Adjust settings with preview&#x20;
* Drag the Performance - Quality slider to 'Quality'.

</details>

<details>

<summary>Broken <code>autoexec.cfg</code> Commands </summary>

Some `autoexec.cfg` commands can break or increase chance of breaking custom DDS skins.

This is pretty rare. I've only heard of this issue happening 4 times.&#x20;

To fix.&#x20;

* Just save your current `autoexec.cfg`
* Create a new blank `autoexec.cfg`&#x20;
* Run the game.
* Close the game.
* Edit `autoexec.cfg` to copy and paste your previous commands.&#x20;

IF THIS DOESN'T WORK. Please share your commands to me for testing but we can get this to work.&#x20;

* Just, copy and paste the commands you want or understand what they do.&#x20;

Minimize the chance of corruption. If not. Just paste the necessities.&#x20;

IF DOESN'T WORK AGAIN.

* Just use a blank `autoexec.cfg` file.&#x20;

If your skins still do not work. Your `autoexec.cfg` is not the issue.

</details>

<details>

<summary>Overlapping Skins</summary>

On certain DDS skins some textures are not included in the release version of the skin resulting in textures from the previous skin not being fully overwritten.&#x20;

* Download needed default textures from [https://github.com/BigSpice/TitanFall-2-Skin-Modding](https://github.com/BigSpice/TitanFall-2-Skin-Modding/tree/main/Textures/Compiled%20textures)
  * If the needed textures aren't there feel free to alert us on discord.
* Install default textures as a skin.
* Reinstall your desired skin.

If this does not work double check if everything installed correctly, if all appears to be good there may be an issue with the skin itself.

</details>
