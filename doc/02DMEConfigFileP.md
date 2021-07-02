# DME-Core Configuration File Protocol
This page describes the DME-Core main configuration file protocol. This file allows the configuration of the DME-Core engine itself.

Each DME-Core add-ons may have its own configuration file.

Essencially the file format is *key* *value*.

Each Keyword (token) in the configuration file is case insenitive, while their values are case sensitive.
Each keyword, when parsed, will be trimmed of spaces surrounding it, but no internal spaces will be touched.
Each keyword value, when parsed, will have surrounding spaces trimmed, but no internal spaces will be touched.

Each line that begins with a "#" symbol is considered a comment and will be ignored.

Protocol example:
```
# DME Section
# This section provides info for the DME-Core Engine to understadn properly the configuration file
# This is useful across different releases of the DME-Core engine
DMEVer: <version of the DME required to process this file> (required)

# Theme Section
# This section allows a user to specify which Theme is selected and needs to be applied at boot
ThemeName: [string]<name of the user select theme> (required)
ThemeVariant: [string]<name of the theme variant if applicable> (optional)

# Wimp Section
# This section contains the lists of what the user has enabled
WindowsFlags: enabled|disabled (this will tell DME-Core to load the Windows Flags configuration add-on)
GlobalControls: enabled|disabled (this will tell DME-Engine to load the Global COntrols configuration add-on)
GlobalGadgets: enabled|disabled (this will tell DME-Core to load the Global Gadgets configuration add-on)

```
