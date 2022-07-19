---
description: very bad docs
---

# Very bad docs

From the R2RePak thread in #research chat in the Northstar Discord

## Type List (for config.json)

gen: the only known use of this is for loadscreens. \
wld: used for map/world materials. \
fix: unsure what this does but in titanfall 2 most materials have a 'fix' counterpart, probably something to do with rendering? \
rgd: no clue tbh. \
skn: this is what models use, so pilots, guns, etc.\


## Subtype List (still for config.json)

for gen: \
loadscreen: this is used for loadscreens (duh). \
wld: none currently.&#x20;

fix: \
viewmodel: full texture set with working emissive texture in first person, but not in the world. \
viewmodel\_skn31: same as above but supports camo usage. \
worldmodel: full texture set with working emissive texture in the world, but not in first person. \
worldmodel\_skn31: same as above but with camo. \
worldmodel\_noglow: full texture set sans emissive. \
worldmodel\_noglow\_skn31: same as above but with camo support.&#x20;

rgd: none currently.&#x20;

skn: \
viewmodel: full texture set with working emissive texture in first person, but not in the world.\
viewmodel\_skn31: same as above but supports camo usage. \
worldmodel: full texture set with working emissive texture in the world, but not in first person.\
worldmodel\_skn31: same as above but with camo. \
worldmodel\_noglow: full texture set sans emissive. \
worldmodel\_noglow\_skn31: same as above but with camo support.&#x20;

visibilityflags: \
opaque: your material will be opaque. \
transparent: your material will be transparent, this does not work out of the box currently. \
colpass: use this if it's a colpass material. \
none: use this if it's a loadscreen material.&#x20;

faceflags: \
6: normal outward drawing faces \
7: outward drawing faces, but wireframe.&#x20;

imageflags: I would avoid messing with these. (for now)

{% hint style="info" %}
saveDebugName does nothing for matls
{% endhint %}

{% hint style="info" %}
ui is in BC7U
{% endhint %}

## Discord Message Links:

[https://discord.com/channels/920776187884732556/987730053439827998/998728801234206772](https://discord.com/channels/920776187884732556/987730053439827998/998728801234206772)[https://discord.com/channels/920776187884732556/987730053439827998/998729837311184896](https://discord.com/channels/920776187884732556/987730053439827998/998729837311184896)[https://discord.com/channels/920776187884732556/987730053439827998/996793988977807410](https://discord.com/channels/920776187884732556/987730053439827998/996793988977807410)



