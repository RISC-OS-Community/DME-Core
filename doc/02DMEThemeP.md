# DME Theme Protocol

## Intro

Each Theme must be created in the way described below to be correctly understood and applied by the DME-Core when the DME-Core calls the Theme-ing Task.

Each Theme is identified by a directory called with the Theme name.
The directory must presents the following structure:

```shell
Theme Name
├── Apps
├── Backgrounds
├── Fonts
├── Palette
├── Pointers
├── Preview
├── Shutdown
├── Sounds
└── Startup
```

## Protocol details

Each theme must contain a configuration file either called Choices or Config.

Essentially the file format is *key* *value*.

Each Keyword (token) in the configuration file is case insensitive, while their values are case sensitive.
Each keyword, when parsed, will be trimmed of spaces surrounding it, but no internal spaces will be touched.
Each keyword value, when parsed, will have surrounding spaces trimmed, but no internal spaces will be touched.

Each line that begins with a "#" symbol is considered a comment and will be ignored.

Protocol Example:

```shell
# Theme data header
Name:The Theme
Info:A theme
Author:The one and only me
License: Apache 2.0
Release:1.0.0
Notes: This theme requires at least 32K display or better

# Theme data

## Desktop Background theming
Backgound:enabled
BackgroundType:1
BackgroundFull:raincode
BackgroundCentred:bridge
BackgroundTile:logo
BackgroundColour:003300

## Windows buttons theming
ButtonSpecial:Yes
ButtonColour:CECEE1
ButtonDefColour:CECEE1
ButtonFade:Yes
ButtonRim:No

BorderThin:No
BorderSpriteIcons:Yes

## General Desktop Theme details
DesktopIcons:Yes
DesktopFontBlend:Yes
3DSettings: No

## Font theming
Font:enabled
FontName:Andale.Mono
FontSize:210
FontWidth:150
FontColour:00ff00

## Hourglass mouse theming
Hourglass:

## Desktop Palette theming
Palette:Dark

## Mouse pointer theming
Pointer:Pointers

## Windows theme-ing
WinTile:Dark
WinTools:Yes
WinHighlight:EDEDFF
WinShade:9999A9
WinOutline:52525C
WinOverwrite:No
WinTextured:Yes
GroupColour:ADB3C1

## Optional if you want a different name for your sprites file
Sprites:Sprites

## Sound theme-ing
SoundOpen:Welcome2
SoundQuit:GetMeOut
Sound00009:<none>
Sound00401:NoiseC
Sound00402:NoiseB
Sound40040:<none>
Sound400C1:<none>
Sound400C2:NoiseB
Sound400C3:Noise2
Sound400CA:NoiseA
Sound400CB:Noise2
Sound400CF:<none>
Sound4AF80:Noise2
SoundError:whoa

## Optional if you want a different name for your tools file
Tool:Tools
```

Lines that starts with an "#" are comments and will be ignored when applying a theme.
