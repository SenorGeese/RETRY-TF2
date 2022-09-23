# Type List

From the R2RePak thread in #research chat in the Northstar Discord by Rika.

```
type list:
	version 12:
		gen: the only known use of this is for loadscreens.
		wld: used for map/world materials.
		fix: unsure what this does but in titanfall 2 most materials have a 'fix' counterpart, probably something to do with rendering?
		rgd: not officially supported in tf|2.
		skn: this is what models use, so pilots, guns, etc.
		
	version 16:
		sknp: todo
		wldc: todo
		gen: todo
	
	usage:
		"type": "string"
	
note: most subtypes are cut because they're no longer needed.
subtype list:
	fix:
		nose_art: used for nose art on titans.
	skn:
		nose_art: used for nose art on titans.
		
		usage:
			"subtype": "string"

visibilityflags:
	opaque: your material will be opaque.
	transparent: your material will be transparent, required for nose art.
	colpass: use this if it's a colpass material.
	none: use this if it's a loadscreen material.
	
	usage:
		"visibilityflags": "string"
	
faceflags:
	6: normal outward drawing faces
	7: outward drawing faces, but wireframe.
	16: this is used for nose art.
	
	usage:
		"faceflags": "HexAsString"
	
flags:
	I would avoid messing with these. However, for the daring see below.
		normal materials: 1D0300
		loadscreens: 50300
		
		usage:
			"flags": "HexAsString"
			
flags2:
	very important stuff. just ask and I will help with the values.
	
	usage:
		"flags2": "HexAsString"
	
emissivetint:
	this is needed if you wish to have an emissive texture, the format is as follows:
		"emissivetint": [rFloat, gFloat, bFloat, aFloat]

albedotint:
	this is set to all '1.0' by default, only change this if you want to adjust the color, the format is as follows:
		"albedotint": [rFloat, gFloat, bFloat, aFloat]
		
uv1transform:
	if you are making a material with a detail/camo texture, the format is as follows:
		"uv1transform": [xScaleFloat, unkFloat, rotationFloat, yScaleFloat, xTransformFloat, yTransformFloat]
		
surface:
	the surface for the material, see scripts/surfaceproperties.txt (titanfall 2) or scripts/surfaceproperties.rson (apex) for a valid surface list.
	
	usage:
		"surface": "string"
		
surface2:
	the same as surface but for edge cases where a secton surface is needed, same list applies.
	
	usage:
		"surface2": "string"
		
height:
	the height of the material.
	
	usage:
		"height": Number
		
width:
	the width of the material.
	
	usage:
		"width": Number
		
path:
	the path of the material, if replacing an existing one this must match said material.
	
	usage:
	 "path": "string"
	 
	example path: "models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31"
	 
colpass:
	the colpass for the material, the path should be the same as whatever you intend to use as your colpass.
	
	usage:
		"colpass": "string"
		
	example path: "models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_colpass"
		
textures:
	this is an array containing strings for the textures you want to use, these must be valid, existing textures within the rpak you a creating.
	there is a certain format to the texture array depending on what you are trying to do and what textures you are using, see below:
	
		slot1 _col
		slot2 _nml 
		slot3 _gls/_exp
		slot4 _spc
		slot5 _ilm
		slot6 never used
		slot7 never used
		slot8 never used
		slot9 never used
		slot10 never used
		slot11 never used
		slot12 _ao
		slot13 _cav/cvt
		slot14 _opa
		slot15 detail/camo
		slot16 _dm_nml/_nml detail normal map
		slot17 _msk detail texture mask
		slot18 special use case
		slot19 special use case
		slot20 special use case
		slot21 never used
		slot22 never used
		the following are used on blend materials, for maps only. it is a second texture to blend into the main one.
		slot23 _bm blendmap
		slot24 _col
		slot25 _nml 
		slot26 _gls/_exp
		slot27 _spc
		
	so, for a material noramlly used on pilots the texture array will look like:
		"textures":[ "_col",
					"_nml",
					"_gls",
					"_spc",
					"_ilm",
					"",
					"",
					"",
					"",
					"",
					"",
					"_ao",
					"_cav" ]

```

## Discord Message Link:

[https://discord.com/channels/920776187884732556/987730053439827998/998777181624877166](https://discord.com/channels/920776187884732556/987730053439827998/998777181624877166)



