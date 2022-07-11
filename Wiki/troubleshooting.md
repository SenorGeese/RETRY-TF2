# Troubleshooting

### General Troubleshooting

<details>

<summary>TF2 Video Settings</summary>

* Open Titanfall 2.
* Navigate to Video settings.
* Check that your 'Texture Filtering' is set to at least 'Anisotropic 8x' (preferably 'Anisotropic 16X').
* Check that your 'Texture Streaming Budget' is sufficient.

</details>

<details>

<summary>Northstar Skin mods</summary>

If the skin is reactive, animated or does something special outside of just basic textures, it's probably installed as a Northstar mod. Check the skin to see if it says to be installed as a mod.

This includes the custom models such as the Cat ears. They are installed as Northstar mods.

You don't need the skin tool for these Northstar mods.

</details>

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

<summary>NVIDIA Control Panel Settings</summary>

\*If you have a Nvidia graphics card.\*

* Open 'NVIDIA Control Panel'
* Navigate to 3D Settings**>>**Adjust settings with preview&#x20;
* Drag the Performance - Quality slider to 'Quality'.

</details>

### Installation Successful but cannot see in-game:

<details>

<summary>Solution 1: NVIDIA Control Panel Settings</summary>

\*If you have a Nvidia graphics card.\*

* Open 'NVIDIA Control Panel'
* Navigate to 3D Settings**>>**Adjust settings with preview&#x20;
* Drag the Performance - Quality slider to 'Quality'.

</details>

<details>

<summary>Solution 2: Broken <code>autoexec.cfg</code> Commands </summary>

Some `autoexec.cfg` commands can break or increase chance of breaking custom DDS skins.

This is pretty rare. I've only heard of this issue happening 4 times.&#x20;

To fix.&#x20;

* Just save your current `autoexec.cfg`

<!---->

* Create a new `autoexec.cfg`

<!---->

* Copy and paste your previous commands.&#x20;

IF THIS DOESN'T WORK. Please share your commands to me for testing but we can get this to work.&#x20;

* Just, copy and paste the commands you want or understand what they do.&#x20;

Minimize the chance of corruption. If not. Just paste the necessities.&#x20;

IF DOESN'T WORK AGAIN.

* Just use a blank `autoexec.cfg` file.&#x20;

If your skins still do not work. Your `autoexec.cfg` is not the issue.

</details>
