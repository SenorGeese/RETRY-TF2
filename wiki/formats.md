---
description: Info about our customizability of skins along side the formats.
---

# Formats

{% hint style="info" %}
These are not the only ways to customize a skin. You can innovate as always. If you feel you made a discovery feel free to share it in the Discord server!
{% endhint %}

## Formats: <a href="#formats" id="formats"></a>

## 2 kinds of skins (VTF format and DDS format) <a href="#2-kinds-of-skins-vtf-format-and-dds-format" id="2-kinds-of-skins-vtf-format-and-dds-format"></a>

### VTF format <a href="#vtf-format" id="vtf-format"></a>

VTF is the first found custom gun skin method. VTF skins are usually in VPKs. Controlled by their VMT files.&#x20;

* Up to 4k skins
* 'Unlimited' view distance
* Only color and normal textures
* Works on low graphics
* Animated skins (VMT options)
* Moving skins (VMT options)
* Transparent skins (VMT options)

### DDS format <a href="#dds-format" id="dds-format"></a>

DDS is the PBR supported custom skins. DDS skins are usually in RPAKs.&#x20;

* PBR or Properly shaded skins
* Community made tools
* High quantity, high-quality skins
* Streamed DDS Skins
  * Limited view distance
  * No transparency
* RePak RPAK DDS Skins
  * 'Unlimited' view distance
  * Transparency

## Format's possibilities <a href="#formats-possibilities" id="formats-possibilities"></a>

### Static, Single frame <a href="#static-single-frame" id="static-single-frame"></a>

Static skins are skins that don't move in any way. Compatible with VTF and DDS format. Simple and at times, most elegant. DDS formats only skin style.

### Moving texture, Single frame <a href="#moving-texture-single-frame" id="moving-texture-single-frame"></a>

Only available with VTF format. Moving skins are skins that have a code group in their `.vmt` that moves your vtf texture to your desired parameters. The code "Proxies"

```
"Proxies"
    {
        "TextureScroll"
        {
            "texturescrollvar" "$baseTextureTransform"
            "texturescrollrate" "-0.03"
            "texturescrollangle" "180"
        }
    }
```

Change `"texturescrollrate" "-0.03"` to change speed of movement. Change `"texturescrollangle" "180"` to change direction of movement.

### Animated texture, Multiple frames <a href="#animated-texture-multiple-frames" id="animated-texture-multiple-frames"></a>

Only available with VTF format. Animated skins are skins that create a moving affect or active scene by using multiple frames. You wont need multiple vtf's as VTFEdit creates one file with every frame inside. Mind that this increases size; which can have affects in recompiling. Note you can use Add-ons on your image editors to help with making animated skins. You need this code group in your models `.vmt` to activate animation; found below.

```
"Proxies"
    {
        "AnimatedTexture"
        {
            "animatedTextureVar"	"$basetexture"
			"animatedTextureFrameNumVar"	"$frame"
			"animatedtextureFrameRate"	"2"
        }
    }
```

### Transparency

Only available with VTF format. Transparency can be enabled in the the model's vmt. Example.

```
$translucent 1
```

### Refract Shader ('mirror')

Only available with VTF format. The refract shader can be apply to give the model a "refracted" look. Documentation here: [https://developer.valvesoftware.com/wiki/Refract](https://developer.valvesoftware.com/wiki/Refract))

```
Refract
{
	$normalmap ...
	$dudvmap ...
	$refracttint "[1 1 1]"
	$refractamount .2
}
```
