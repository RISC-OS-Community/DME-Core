# DME-Core Requirements

## As a RISC OS user I would like that:
RU0001
______
The DME-Core Engine should be able to set:
- Theme preferences
- Windowing Configurations (Windows FLags)
- Load user activated Global Controls
- Load user activated Desktop Gadgets

RU0002
______
To fulfill R00001 it should read a configuration file that can be modified by the user using the DME ConfigTools.
The configuration file:
- should reside in !Boot:Choices.DME
- Should be a set of configurations files (or just one)?
- It should be following a well define configuration protocol (see 01DMEConfigFileP/txt for details)

RU0003
______
Every add-on (Global Controls, Theme, Gadget) should be enabbled or disabled via an option on the Configuration UI.

RU0004
______
For new users there should be an "initial configuration" available as a "Wizzard Process" where they could set up the RISC OS withough the need to know where to go and what to do. A bit like it works on every Apple devices where at the first boot a user is asked to "customise" their device.

## As a RISC OS Vendor I would like that:
RV0001
______
I could customise my devices with my own Theme and have it easy to do so (like just copying a config directory in Boot:Choices)

RV0002
______
I would like to be able to control the "Initial Configuration Process" by setting which steps a user could perform on my devices

## As a RISC OS Developer/Theme Creator I would like that
RD0001
______
I could use some Wimp Tool to be able to create a Theme instea dof having to do everything manually

RD0002
______
I would like to have an easy way to distribute my Theme and for the users to install it on their devices

RD0003
______
I would liek that the Theme System would work on as many RISC OS devices and RISC OS releases as possible in order to maximise the distribution of my work
 
