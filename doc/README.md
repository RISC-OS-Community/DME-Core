# DME-Core documentation
This is the "ConfigurationObject" for the entire DME.

It reads all the configuration files, the Operating System version and the Window version and applies a desired configuration accordingly.

## Requirements
[Detailed requirement list here](00DMERequirements.md)

## Design
[DME Design is available here](01DMEDesign.md)

## DME Config File Protocol
[DME Configuration File Protocol details available here](02DMEConfigFileP.txt)

## DME Theme Protocol
The DME Theme Protocol is inspired by Rich Goodwin and Chir (Little Yellow Moon) works.
It foundamentally is a text file that describes all the options and details to apply a theme correctly (where correctly means "as the original theme author meant it to be applied")

This type of feature does not exists in the bare RISC OS and so must be added in order to make DME be able to deal with complex themes that may require more than just reload the tool sprites.

[Details on the Theme Protocol available here](02DMEThemeP.txt)
