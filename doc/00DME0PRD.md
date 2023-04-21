# Product Requirements Document

## As a RISC OS user I would like that

*RU0001*

The DME-Core Engine should be able to set:

* Theme preferences
* Windowing Configurations (Windows FLags)
* Load user activated Global Controls
* Load user activated Desktop Gadgets

------

*RU0002*

To fulfill RU0001 it should read a configuration file that can be modified by the user using the DME ConfigTools.
The configuration file:

* Should reside in !Boot:Choices.DME
* Should be either a set of configurations files or just a single file
* It should be following a well define configuration protocol ([see here for more details](02DMEConfigFileP.md))

------

*RU0003*

Every add-on (Global Controls, Theme, Gadget) should be enabled or disabled via an option on the Configuration UI.

------

*RU0004*

For new users there should be an "Initial Configuration" available as a "Wizard Process" where they can set up RISC OS without the need to know where to go and what to do. A bit like it works on every Apple device where at the first boot a user is asked to "customise" their device.

------

## As a RISC OS Vendor I would like that

*RV0001*

I can customise my devices with my own Theme and have an easy way to do so (like just copying a config directory in Boot:Choices)

------

*RV0002*

I would like to be able to control the "Initial Configuration Process" by setting which steps a user can perform on my devices

------

## As a RISC OS Developer/Theme Creator I would like that

*RD0001*

I can use some Wimp Tool to be able to create a Theme instead of having to do everything manually

------

*RD0002*

I would like to have an easy way to distribute my Theme and for the users to install it on their devices

------

*RD0003*

I would like that the Theme System would work on as many RISC OS devices and RISC OS releases as possible in order to maximise the distribution of my work. Possibly the Theme System should recognise each release of RISC OS and apply my Theme in a way that makes it compatible with the specific version.

------
