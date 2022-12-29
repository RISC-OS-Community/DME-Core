# DME Technical Requirements Document

## General requirements

1. DME should be designed and developed supporting the following RISC OS releases:

        OS Release                    |  ARM Arch
        ----------------------------- | -----------
        From RISC OS 3.10 to 3.71     | (26 bit)
        From RISC OS 4.02 TO 4.39     | (26 bit)
        RISC OS 6.10                  | (26/32 bit)
        From RISC OS 5.28 onward      | (32 bit)

2. Code should be written in a high level programming language as C, BBC BASIC, Lua etc. giving priority to languages that are fully supported on RISC OS and possibly executable on all supported RISC OS versions.

3. Code should be written to be testable and tests (where applicable) should be included with the code.

4. Code should be written to be "build-able" on a 3rd party RISC OS device, in other words, no customizations of build environment should be done and the build should be designed so it can be executed also on GitHub pipelines.

5. For compiled code, it should be built so that it can work on all releases of RISC OS mentioned at point 1.

6. While it would be great if every single components of the DME would run on all RISC OS versions and all the old platforms, the developer should always consider that features and code stability come first, so when something cannot be made for older versions of RISC OS or old platforms in order to achieve better functionalities and stability then such code should be designed focusing on the modern platforms only.

7. Each component should be always designed having in mind the following parts:

        Part                      |  Description
        ------------------------- | ----------------------------------------
        Provide useful features   |  Each component should always provide
                                  |  useful features to the end user, the
                                  |  hardware vendor, other developers.
        ------------------------- | ----------------------------------------
        Extend OS functionalities |  Each component should always extend
                                  |  the OS functionality through an API.
                                  |  Such API should be provided either
                                  |  as an SWI set (if the component is
                                  |  executable as a single task element)
                                  |  OR via WIMP Messages (if the component
                                  |  is executable ONLY in the WIMP).
        ------------------------- | ----------------------------------------
        Follow the RISC OS Style  |  Each component should be designed 
        Guide                     |  following the RISC OS Style Guide rules
                                  |  where applicable and define new rules
                                  |  where the Style guide lack such or is
                                  |  confusing on the specifics.
        ------------------------- | ----------------------------------------
        Integrate with other DME  |  Where applicable, each DME component
        Components                |  should be designed to integrate with
                                  |  other DME components and the existing
                                  |  one on the OS. This in order to avoid
                                  |  duplication of logic.
        ------------------------- | ----------------------------------------
