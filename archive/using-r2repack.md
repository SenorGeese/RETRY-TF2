# How to use R2RePak

From the R2RePak thread in #research chat in the Northstar Discord by Spoon. This is the archive of the pseudo guide. Discord Message Link at the bottom of the page.

This is no longer the original guide. This is now an edited version of pseudo guide.

## **Setting things up**&#x20;

### 1 ) Build RePak or Download RePak.

You can build from [https://github.com/ASpoonPlaysGames/RePak/tree/R2-not-bad](https://github.com/ASpoonPlaysGames/RePak/tree/R2-not-bad).

or Download the from the Releases page on the Github; [https://github.com/ASpoonPlaysGames/RePak/releases](https://github.com/ASpoonPlaysGames/RePak/releases).

But this guide will use the .zips names and config below.

{% file src="../.gitbook/assets/RePak-edited-1.0.0.zip" %}

### 2 ) Project Folders

In the folder where you have RePak.exe we have a folder called "assets" a folder called "config" and a folder called "rpaks"

the "assets" folder is where you will put your folder/file structure and textures etc.&#x20;

the "config" folder is where you will put the .json files which determine how the rpak is made&#x20;

&#x20;the "rpaks" folder is where RePak will put the rpaks once they have been made&#x20;

### 3 ) Make pack\_all.bat

&#x20;in the folder with RePak.exe, make a .bat file, i called mine "pack\_all.bat".&#x20;

Inside the .bat put

```
for %%i in ("%~dp0config\*") do "%~dp0RePak.exe" "%%i"
pause
```

## **Making your rpaks**&#x20;

### 1 ) Make .json

&#x20;Make the .json file, give it a name, here it's named `config.json`.

### 2 ) Copy and paste in your .json

go into the json file, and copy the following into it for now

```
{
    "name":"common",
    "assetsDir":"../assets",
    "outputDir":"../rpaks",
    "files":[
        {
            "$type":"txtr",
            "path":"texture/models/titans_r2/light_ronin/nose_art/nose_art_v14/t_l_ronin_nose_art_v14_col",
            "saveDebugName": false
        },
        {
            "$type":"txtr",
            "path":"texture/models/titans_r2/light_ronin/nose_art/nose_art_v14/t_l_ronin_nose_art_v14_opa",
            "saveDebugName": false
        }
        ,
        {
            "$type":"txtr",
            "path":"texture/models/titans_r2/light_ronin/nose_art/nose_art_v14/t_l_ronin_nose_art_v14_gls",
            "saveDebugName": false
        }
        ,
        {
            "$type":"txtr",
            "path":"texture/models/titans_r2/light_ronin/nose_art/nose_art_v14/t_l_ronin_nose_art_v14_spc",
            "saveDebugName": false
        }
    ]
}
```

{% hint style="info" %}
if your output folder and your asset folder have different names, be sure to change the "assetsDir" and "outputDir" respectively&#x20;
{% endhint %}

This is set up now to make a ronin nose art, you can change the paths in the .json to make it override other things. I removed everything but the \_col map.

You can get the paths for things through Legion+.

### 3 ) Use your textures

For each entry in the json file, you need to make sure that the file exists in the assets folder so it can be packed.&#x20;

Textures must be in .dds format, and with one of the following compression methods: \
DXT1 \
BC4U \
BC5U \
DX10&#x20;

### 4 ) Packing your rpak

To pack your rpaks, run `pack_all.bat`&#x20;

### 5) Resources

Here is the working test.

{% file src="../.gitbook/assets/RePak-guide-1.0.0.rar" %}

## **Making the Northstar mod**&#x20;

### 1 ) Northstar mod set up

Take your rpak, and make your Northstar mod like normal, inside the Northstar mod, make a "paks" folder.

### 2 ) Make rpak.json

Within the "paks" folder, make a json file called `rpak.json` .

### 3 ) Copy and paste in rpak.json

&#x20;put the following into the rpak.json:

```
{
    "Preload": {
        "common.rpak": true
    }
}
```

{% hint style="info" %}
if your rpak is called something other than `common.rpak` make sure the json file reflects that&#x20;
{% endhint %}

### 4 ) Drag & Drop

Drag and drop your rpak into the "paks" folder.

{% file src="../.gitbook/assets/dev-RePakTest.rar" %}
This guides Included Test .rar file.
{% endfile %}

{% file src="../.gitbook/assets/RPak.Tests.zip" %}
Included Test .zip file (doesn't belong to this guide)
{% endfile %}

### Discord Message Link:

[https://discord.com/channels/920776187884732556/987730053439827998/988111160786190386](https://discord.com/channels/920776187884732556/987730053439827998/988111160786190386).

### Things that might be useful:

Glitch Loadscreen Change: [https://discord.com/channels/920776187884732556/987730053439827998/988136914819354654](https://discord.com/channels/920776187884732556/987730053439827998/988136914819354654)

ReDecompress (decompress rpak files): [https://github.com/IcePixelx/ReDecompress](https://github.com/IcePixelx/ReDecompress)

