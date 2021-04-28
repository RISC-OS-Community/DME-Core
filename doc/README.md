# DME-Core documentation
This is the "ConfigurationObject" for the entire DME.

It reads all the configuration files, the Operating System version and the Window version and applies a desired configuration accordingly.

## "Business" Requirements Document (BRD)
All the code in this community is distributed as Open Source and so the word business goes a bit between "", however the BRD is an important document that describes what we want to achieve and which problem do we want to solve with the DME project.

[Detailed BRD here](00DME0BRD.md)

## Market Requirements Document (MRD)
RISC OS is an Operating System that at the moment has the advantage of being extremely minimalistic. This is definitely an advantage in markets like IoT and Embeeded Applications, however improving its desktop functionalities would certainly help those who wish to adopt RISC OS for their own solutions development.
Having a more modern experience and a more standardised one will certainly help to reduce the initial learning curve to adopt RISC OS as a platform for developing and distributing 3rd party applications and solutions.

[Detaled MRD here](00DME0MRD.md)

## Product Requirements Dcument (PRD)
This document is what most users are interested to:

[Detailed PRD here](00DME0PRD.md)

## Technical Requirements Document (TRD)
This document contains all the details about the DME requirements in terms of supported platforms, releases of RISC OS and required resources to run smoothly on a system.

We'd recommend to read it before installing and using the DME Engine on your RISC OS system and/or platform.

[detailed TRD here](00DME0TRD.md)

## Design
[DME Design is available here](01DMEDesign.md)

### DME Config File Protocol
[DME Configuration File Protocol details available here](02DMEConfigFileP.md)

### DME Theme Protocol
The DME Theme Protocol is inspired by Rich Goodwin's and Chir's (Little Yellow Moon) works.
It is fundamentally a text file that describes all the options and details to apply a theme correctly (where correctly means "as the original theme author meant it to be applied")

This type of feature does not exists in the bare RISC OS and so must be added in order to make DME be able to deal with complex themes that may require more than to just reload the tool sprites.

[Details on the Theme Protocol available here](02DMEThemeP.md)

