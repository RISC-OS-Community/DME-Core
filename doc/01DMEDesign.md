# DME-Core
The DME-Core is a RISC OS App that contains both logic and resources to achieve the requirement goals.

DME-Core Directory structure:
```
!DMECore
├── Resources
│   └── UK
└── Store
    ├── Controls
    ├── Gadgets
    └── Themes
```
The Resources directory is the standard RISC OS repository for territory and messages as well as app templates (if neeved)

The Store directory contains all the Global Controls, Gadgets and Themes repositories.

The !DMECore app contains a !RunImage file which, when executed, will read:
* The Operating System version
* The Window Module version
* The Main Configuration file stored in Boot:Choices.DME [more details about it here](02DMEConfigFileP.md) 
And it will apply all the changes accordingly (in the futures it may also apply RISC OS Patches required by advnaced functionalities).

The !DMECore should be capable of applying the above on demand and without the need to reboot the system.
