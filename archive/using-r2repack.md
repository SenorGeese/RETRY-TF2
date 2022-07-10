# How to use R2RePak

From the R2RePak thread in #research chat in the Northstar Discord by Spoon. This is the archive of the pseudo guide. Discord Message Link at the bottom of the page.

## **Setting things up**&#x20;

### 1 ) Build RePak

You can build from [https://github.com/ASpoonPlaysGames/RePak/tree/R2-not-bad](https://github.com/ASpoonPlaysGames/RePak/tree/R2-not-bad).

### 2 ) Project Folders

in the folder where you have RePak.exe make a folder called "assets" a folder called "maps" and a folder called "rpaks" (the names dont really matter tbh)&#x20;

the "assets" folder is where you will put your file structure and textures etc.&#x20;

the "maps" folder is where you will make json files which determine how the rpak is made

&#x20;the "rpaks" folder is where RePak will put the rpaks when they have been made&#x20;

### 3 ) Make pack\_all.bat

&#x20;in the folder with RePak.exe, make a .bat file, i called mine "pack\_all.bat".&#x20;

Inside the .bat put

```
for %%i in ("%~dp0maps\*") do "%~dp0RePak.exe" "%%i"
pause
```

make sure if you used a different name for the maps folder you replace "maps" in the bat file&#x20;

## **Making your rpaks**&#x20;

### 1 ) Make .json

&#x20;Make the .json file, give it a name, doesnt rly matter what it is&#x20;

### 2 ) Copy and paste in your .json

go into the json file, and copy the following into it for now

```
{
    "name":"common",
    "assetsDir":"../depot",
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

This is set up now to make a ronin nose art, you can change the paths in the .json to make it override other things. You can get the paths for things through Legion+.

### 3 ) Use your textures

For each entry in the json file, you need to make sure that the file exists in the assets folder so it can be packed.&#x20;

Textures must be in .dds format, and with one of the following compression methods: \
DXT1 \
BC4U \
BC5U \
DX10&#x20;

### 4 ) Packing your rpak

to pack your rpaks, run `pack_all.bat`&#x20;

## **Making the Northstar mod**&#x20;

### 1 ) Northstar mod set up

Take your rpak, and make your Northstar mod like normal, inside the Borthstar mod, make a "paks" folder.

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

### 4 ) Yup

Drag and drop your rpak into the "paks" folder.

{% file src="../.gitbook/assets/RPak.Tests.zip" %}
Included Test .zip file.
{% endfile %}

### Discord Message Link:

[https://discord.com/channels/920776187884732556/987730053439827998/988111160786190386](https://discord.com/channels/920776187884732556/987730053439827998/988111160786190386).

### Things that might be useful:

Glitch Loadscreen Change: [https://discord.com/channels/920776187884732556/987730053439827998/988136914819354654](https://discord.com/channels/920776187884732556/987730053439827998/988136914819354654)

ReDecompress (decompress rpak files): [https://github.com/IcePixelx/ReDecompress](https://github.com/IcePixelx/ReDecompress)

