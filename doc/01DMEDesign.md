# DME-Core

The DME-Core is a RISC OS App that contains both logic and resources to achieve the requirement goals.

DME-Core Directory structure:

```shell
!DeskRes
├── Resources
│   └── UK
├── DME
│   ├── Components
│   ├── Gadgets
│   └── Plugins
├── Scripts
│   ├── Autostart
│   └── Setup
.
.
.
```

The Resources directory is a standard RISC OS repository for territory and messages as well as app templates (if needed)

The DME directory contains all the Global Components, Gadgets and Plugins repositories.

A Component in the DME can be an applications, module or task-module that provides a well defined functionality from the list of macro functionalities defined by the DME architecture.

A Gadget if an Application that uses directly such functionalities to provide a WIMP user-interface to access and use one or more components, if a components doesn't provides a direct UI (User Interface).

A Plugin is generally an piece of software that uses Acorn Plugin protocol to extend the functionalities of either a COmponent or a Gadget.

A Dependency is a pieces of software (generally either a Module or a software Library) required by one or more of the above components.

The !DeskRes app contains a !RunImage file which, when executed, will read:

* The Operating System version
* The Window Module version
* The Main Configuration file stored in Boot:Choices.DME [more details about it here](02DMEConfigFileP.md) 

And it will apply all the changes accordingly (in the futures it may also apply RISC OS Patches required by advanced functionalities).

!DeskRes also provides a way to "Autostart" a user selected set of Components and Gadgets (and their dependencies)

The !DeskRes should be capable of applying the above on demand and without the need to reboot the system (where possible).
