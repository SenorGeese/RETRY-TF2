---
layout: landing
---

# Working Materials Examples

### Normal Material

{% code title="beta_pulse.json" %}
```json
{
    "name": "betapulse",
    "assetsDir": "E:/titanfall/projects/rpak/repak/assets",
    "outputDir": "E:/titanfall/projects/rpak/repak/rpaks",
	"version": 7,
    "files":[
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_col",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
            "$type":"matl",
			"version":12,
			"type": "fix",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_colpass",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"shaderset": "uberAoCavEmitEntcolmeSamp2222222_fix",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav" ],
			"visibilityflags": "colpass",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56000020",
			"width": 4096,
			"height": 2048,
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
            "$type":"matl",
			"version":12,
			"type": "fix",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"colpass": "models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_colpass",
			"shaderset": "uberAoCavEmitEntcolmeSamp2222222_fix",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav" ],
			"visibilityflags": "opaque",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56000020",
			"width": 4096,
			"height": 2048,
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
            "$type":"matl",
			"version":12,
			"type": "skn",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_colpass",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"shaderset": "uberAoCavEmitEntcolmeSamp2222222_skn",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav" ],
			"visibilityflags": "colpass",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56000020",
			"width": 4096,
			"height": 2048,
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
            "$type":"matl",
			"version":12,
			"type": "skn",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"colpass": "models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_colpass",
			"shaderset": "uberAoCavEmitEntcolmeSamp2222222_skn",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav" ],
			"visibilityflags": "opaque",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56000020",
			"width": 4096,
			"height": 2048,
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_col",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_msk",
			"starpakpath": "betapulse_hotswap.starpak",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/models/camo_skins/camo_skin01_col",
			"saveDebugName": true	
		},
		{
            "$type":"matl",
			"version":12,
			"type": "fix",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_colpass",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"shaderset": "uberAoCavEmitDetovrDtmEntcolmeUV2000000010Samp222222222_fix",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav",
			"",
			"texture/models/camo_skins/camo_skin01_col",
			"",
			"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_msk" ],
			"visibilityflags": "colpass",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56040020",
			"width": 4096,
			"height": 2048,
			"uv1transform": [4.0, 0.0, -0.0, 4.0, 0.0, 0.0],
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
            "$type":"matl",
			"version":12,
			"type": "fix",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"colpass": "models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_colpass",
			"shaderset": "uberAoCavEmitDetovrDtmEntcolmeUV2000000010Samp222222222_fix",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav",
			"",
			"texture/models/camo_skins/camo_skin01_col",
			"",
			"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_msk" ],
			"visibilityflags": "opaque",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56040020",
			"width": 4096,
			"height": 2048,
			"uv1transform": [4.0, 0.0, -0.0, 4.0, 0.0, 0.0],
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
            "$type":"matl",
			"version":12,
			"type": "skn",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_colpass",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"shaderset": "uberAoCavEmitDetovrDtmEntcolmeUV2000000010Samp222222222_skn",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav",
			"",
			"texture/models/camo_skins/camo_skin01_col",
			"",
			"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_msk" ],
			"visibilityflags": "colpass",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56040020",
			"width": 4096,
			"height": 2048,
			"uv1transform": [4.0, 0.0, -0.0, 4.0, 0.0, 0.0],
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        },
		{
            "$type":"matl",
			"version":12,
			"type": "skn",
			"subtype": "",
			"surface": "default",
            "path":"models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31",
			"materialrefs": [ "code_private/depth_shadow", "code_private/depth_prepass", "code_private/depth_vsm" ],
			"colpass": "models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_colpass",
			"shaderset": "uberAoCavEmitDetovrDtmEntcolmeUV2000000010Samp222222222_skn",
			"textures":[ "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_col",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_nml",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_gls",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_spc",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_02_ilm",
            "",
            "",
            "",
            "",
            "",
            "",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_ao",
            "texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_03_cav",
			"",
			"texture/models/camo_skins/camo_skin01_col",
			"",
			"texture/models/humans/titanpilot_gsuits/pilot_medium_v_helmets/pilot_med_helmet_v1_skn_31_msk" ],
			"visibilityflags": "opaque",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "56040020",
			"width": 4096,
			"height": 2048,
			"uv1transform": [4.0, 0.0, -0.0, 4.0, 0.0, 0.0],
			"albedotint": [ 1.0, 1.0, 1.0],
			"emissivetint": [ 1.0, 1.0, 1.0]
			
        }
    ]
}
```
{% endcode %}

### World Material

{% code title="world_test.json" %}
```json
{
    "name": "worldtest",
    "assetsDir": "E:/titanfall/projects/rpak/repak/assets",
    "outputDir": "E:/titanfall/projects/rpak/repak/rpaks",
	"version": 7,
    "files":[
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_02_col",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/detail_warp01",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_02_gls",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_02_spc",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_02_opa",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/water_droplets_01_col",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/water_droplets_03_nml",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_03_bm",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_03_col",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_03_nml",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_03_gls",
			"saveDebugName": true	
		},
		{
			"$type": "txtr",
			"path":	"texture/world/timeshift/windows/ts_window_destroyed_03_spc",
			"saveDebugName": true	
		},
		{
            "$type":"matl",
			"type": "wld",
			"subtype": "",
			"surface": "glass",
			"surface2": "glass",
            "path":"world/timeshift/windows/ts_window01_dark_cracked_bm",
			"materialrefs": [ "", "", "" ],
			"shaderset": "uberLyrDetallOpamDetDtnTransUV4010002200000Samp222222222222_wld",
			"textures":[ "texture/world/timeshift/windows/ts_window_destroyed_02_col",
						"texture/world/timeshift/windows/detail_warp01",
						"texture/world/timeshift/windows/ts_window_destroyed_02_gls",
						"texture/world/timeshift/windows/ts_window_destroyed_02_spc",
						"",
						"",
						"",
						"",
						"",
						"",
						"",
						"",
						"",
						"texture/world/timeshift/windows/ts_window_destroyed_02_opa",
						"texture/world/timeshift/windows/water_droplets_01_col",
						"texture/world/timeshift/windows/water_droplets_03_nml",
						"",
						"",
						"",
						"",
						"",
						"",
						"texture/world/timeshift/windows/ts_window_destroyed_03_bm",
						"texture/world/timeshift/windows/ts_window_destroyed_03_col",
						"texture/world/timeshift/windows/ts_window_destroyed_03_nml",
						"texture/world/timeshift/windows/ts_window_destroyed_03_gls",
						"texture/world/timeshift/windows/ts_window_destroyed_03_spc" ],
			"visibilityflags": "transparent",
			"faceflags": "6",
			"flags": "1D0300",
			"flags2": "72000002",
			"width": 512,
			"height": 512,
			"albedotint": [ 1.0, 0.0, 0.0, 1.0 ]
			
        }
    ]
}
```
{% endcode %}
