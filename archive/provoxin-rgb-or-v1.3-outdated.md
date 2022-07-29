---
description: A guide on how to use Provoxin RGB V1.3 for team lights
---

# Provoxin RGB | V1.3 (Outdated)

{% hint style="warning" %}
Editing this way will _**not**_ effect your game when running vanilla
{% endhint %}

Firstly you will need to have Provoxin RGB installed onto Northstar, I will assume you know how to install a Northstar mod or already have the mod installed.

{% embed url="https://github.com/Provoxin/Provoxin.RGB/releases/tag/v1.3" %}
**Github link to download page for Provoxin RGB**
{% endembed %}

Before we can do anything we will need a few tools, don't worry, you won't need to install anything. Open a color picker online alongside this converter.

{% embed url="http://hewmc.blogspot.com/2012/12/rgb-to-percentage-converter.html" %}
**Hex/RGB to percent converter**
{% endembed %}

{% embed url="https://coolors.co/color-picker" %}
**Color picker**
{% endembed %}

### Disabling Color cycling

{% hint style="info" %}
If you have already disabled color cycling you can skip right to the next part
{% endhint %}

Open the Provoxin RGB mod folder (in `\Titanfall2\R2Northstar\mods`) and open `mod.json` you will see some switches, I'll walk you through the most important ones. \
\
`"Name": "rgb_ally_rainbow"` \
`"DefaultValue": "1"` \
This controls whether or not allies will cycle through colors, here you're going to set the default value to `"0"`\
\
`"Name": "rgb_enemy_rainbow"` \
`"DefaultValue": "1"` \
This controls whether or not enemies will cycle through colors, here you will also set the default value to `"0"`\
\
Save the `mod.json`

### Changing the colors <a href="#changing-the-colors" id="changing-the-colors"></a>

Next we're going to need a color, open your color picker and choose any color, I'd advise to _**not**_ use a very saturated color, darker colors work the best.

Once you've found the color you want to use in my case that would be "**#336F2D**" in hex and "**51 111 45**" in RGB, open the the hex/RGB to percent converter. Type in the hex or RGB code of your color into the converter, set "number of digits" to 3, and convert.

![Remove any special characters when typing in your values](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FpfSQGjBs3J0Y0NH50na3%2Fuploads%2FGzKGrzq7jfrB3vDY8iVg%2Fimage.png?alt=media\&token=82f60a10-2b10-48d0-9b10-8976a4094d4f)

Click your way through the `mod` folder until you find `rgb.nut`. You will once again see a bunch of code, but what we're interested in are these two lines.

{% hint style="info" %}
The "8" at the end of all the values are brightness, although it's best to leave it be
{% endhint %}

{% code title="rgb.nut" %}
```squirrel
const array<string> DEFAULT_ALLY_COLORS = [ "0.34 0.59 0.86 8", "0.24 0.50 0.96 8", "0.0 0.58 0.77 8", "0.28 0.52 0.97 8" ];
const array<string> DEFAULT_ENEMY_COLORS = [ "0.8 0.25 0.15 8", "0.89 0.78 0.0 8", "1.0 0.627 0.68 8", "0.82 0.74 0.06 8" ];
```
{% endcode %}

These lines are the default colors for all the the colorblind options for allies and enemies, these values are what we're going to be changing.

The values are in chronological order to the colorblind options in-game;\
<mark style="color:blue;">`"0.34 0.59 0.86 8"`</mark> <mark style="color:red;">`"0.8 0.25 0.15 8"`</mark> is "Off" \
<mark style="color:blue;">`"0.24 0.50 0.96 8"`</mark> <mark style="color:red;">`"0.89 0.78 0.0 8"`</mark> is "Protanopia"\
<mark style="color:blue;">`"0.0 0.58 0.77 8"`</mark> <mark style="color:red;">`"1.0 0.627 0.68 8"`</mark> is "Deuteranopia" \
<mark style="color:blue;">`"0.28 0.52 0.97 8"`</mark> <mark style="color:red;">`"0.82 0.74 0.06 8"`</mark> is "Tritanopia" \
\
Simply replace the value of your desired colorblind option in `rgb.nut` with the new values the converter spew out.

{% hint style="success" %}
Aaaaand boom, now go on and enjoy your new beautiful lights! <3
{% endhint %}

![wew so pretty!](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FpfSQGjBs3J0Y0NH50na3%2Fuploads%2FJfQNQEf0nBzeYSKBvAcR%2Faaaaaaa%20green%20lighs%20ig.png?alt=media\&token=1494a08c-d2de-40e5-a183-b77804086027)
