# Hex locating textures.

From the pins in #skins-chat in the Northstar Discord by Creamy. This is the archive of the pseudo guide. Discord Message Link at the bottom of the page.

## Content:

If you still have trouble pinpointing which texture are you looking at based on the avaible diagram, do the following:

1. Go to: [https://web.archive.org/web/20210725135838/https://gist.githubusercontent.com/mrsteyk/f9f853d93139cd395c1a49ab24b17b3d/raw/fdae77196a8f861c03373b243573096bd88406c0/common.rpak.log](https://web.archive.org/web/20210725135838/https://gist.githubusercontent.com/mrsteyk/f9f853d93139cd395c1a49ab24b17b3d/raw/fdae77196a8f861c03373b243573096bd88406c0/common.rpak.log)
2. Initiate search via: ctrl+f and paste in entire name of the texture (i.e. 0x4bf97eea964478bc)
3. This is what you are looking for:\
   models\Weapons\_R2\p2011\_pstl\P2011\_pstl\_colpass.60156591C09BEEB1.matl | weapon\
   Desc@000000000C63B61E size 0xD0 \
   Data@000000000CD70D86 \
   Ref: 0x4BF97EEA964478BC | \_col <-- in our example this will be highlighted \
   Ref: 0x421F263E6960457E | \_nml \
   Ref: 0x8439E7F9E1190442 | \_gls \
   Ref: 0xB0ECC3052B39F265 | \_spc \
   Ref: 0x7B8EFD2AC4A62D7 | \_ilm \
   Ref: 0x0 | UNK5 Ref: 0x0 | UNK6 \
   Ref: 0x0 | UNK7 Ref: 0x0 | \_bm \
   Ref: 0x0 | UNK9 Ref: 0x0 | UNK10 \
   Ref: 0x4712D838BB12430A | \_ao \
   Ref: 0x5BFB1A1096F39EC9 | \_cav
4. and remember: \
   col= color/diffuse map \
   spc= specular map \
   nml= normal map \
   gls= glossiness map \
   ilm= illumination/emmisive map \
   ao= ambient occlusion map \
   cav= cavity map

{% embed url="https://cdn.discordapp.com/attachments/928271573977296957/933459114938486864/assets2F-LPXG6BIVWwbrvVSOiBw2F-MENY3jTkkMuOHfbXj7a2F-MENmQnjhqnPQzGkBcd_2FTexture-linking.png" %}

{% hint style="info" %}
or This corrected and better texture map below!
{% endhint %}

![](../.gitbook/assets/texturemap.png)

### Discord Message Link:

[https://discord.com/channels/920776187884732556/928271573977296957/933459114804260884](https://discord.com/channels/920776187884732556/928271573977296957/933459114804260884).
