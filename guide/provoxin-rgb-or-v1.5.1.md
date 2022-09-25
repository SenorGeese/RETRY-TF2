---
description: A guide on how to use Provoxin RGB
---

# Provoxin RGB | V1.5.1

{% hint style="warning" %}
Editing this way will not effect your game when running vanilla
{% endhint %}

Firstly you will need to have Provoxin RGB installed onto Northstar, I will assume you know how to install a Northstar mod or already have the mod installed.&#x20;

{% embed url="https://github.com/H0L0theBard/Provoxin.RGB/releases/tag/v1.5.1" %}
**Download link for Provoxin RGB**
{% endembed %}

### Disabling color cycling <a href="#disabling-color-cycling" id="disabling-color-cycling"></a>

{% hint style="info" %}
If you have already disabled color cycling you can skip right to the next part
{% endhint %}

Launch the Northstar client and firstly check if the mod was installed correctly by looking in the mods tab. If installed correctly press `"Launch Northstar"` and you should see your pilot and titan cycling through colors.

Open the command window with `` ` ``; which can be complicated if you're not using an American keyboard layout, like me. If you don't use a US keyboard, rebind `"Toggle Developer Console"` to one of the function keys `"F1-F12"` If you cannot find the setting please refer to the R2Northstar wiki.&#x20;

{% embed url="https://r2northstar.gitbook.io/r2northstar-wiki/using-northstar/commands#rebinding-the-console" %}
**Official Northstar wiki | Rebinding the console**
{% endembed %}

Once you've gotten the developer console open write the commands;

`rgb_ally_rainbow 0`

`rgb_enemy_rainbow 0`

Your pilot and titan should stop cycling through colors and show the colors of your selected colorblind option.

### Changing the colors <a href="#changing-the-colors" id="changing-the-colors"></a>

Firstly pick a color from a color picker and grab its RGB value.&#x20;

{% embed url="https://coolors.co/color-picker" %}
**Online Color picker**
{% endembed %}

Write in the command(s) into the developer console;

`rgb_ally_color [RGB value] [Brightness]` For allied colors.

`rgb_enemy_color [RGB value] [Brightness]` For enemy colors.&#x20;

<details>

<summary>Example</summary>

`rgb_ally_color 19 35 123 8`

`rgb_enemy_color 235 27 48 12`

</details>

{% hint style="success" %}
Enjoy your new pretty lights <3
{% endhint %}

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbENNhHo9Z866uxlHGFmT%2Fuploads%2FsCeG1Cux7zjfpUSyEjwK%2Faaaaaaa%20green%20lighs%20ig.png?alt=media&#x26;token=1494a08c-d2de-40e5-a183-b77804086027" alt=""><figcaption><p><strong>Wew so pretty!!</strong></p></figcaption></figure>
