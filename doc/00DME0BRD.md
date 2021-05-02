# Business Requirements Document

## Project overview

One of the first element of a  Modern Operating System that is perceived by any type of user is the usability of its interaction environment (either command line based or graphical user interface based).

Regardless the technologies implied in the general architecture of the OS or the number of applications it can be used for, the interaction with such device or operating system is the very first element a user will always perceive.

On top of that the user interface (UI) can also make (or break) the productivity that an Operating System (OS) offers to users of every type.

Finally in modern times general (and non general) users are exposed to a lot of different OS compared to what used to happen back in the early days of home computing pioneers and so they have developed expectations and perceptions towards how interaction with modern computers and OS should happens.

RISC OS has received little to none improvement and refactor to follow the new trends on the matter of UI and so we thought it would be very useful to introduce a way to allow such changes to be applicable to the RISC OS UI in order to improve and facilitate new users experience on our beloved OS.

At the same time such changes shall not be invasive and shall kept optional so that old userbase still affectinated to the old way RISC OS had to interact with the user.

## Success factors

We'd define as success factors for this project the possibility for a new user to define and use an environment and UI as close as possible to "the modern perceptions created by far more popular OS like MS Windows and Apple macOS". While older users acustomed to the old UI shall be let free to keep using the OS as they liked it to be.

Another success factor would be that new users and old user would have an extremely easy way to achieve their UI configuration goals that would require little to no knowledge of RISC OS for the new users and little to no knowledge of the new UI from older users.

## Project Scope

This project has no intention to modify the Operating System internals. In a first phase it should be limited to work to add the required tools to achieve the goals in the overview and, eventually, in a second phase it may be sligthely more invasive, but only from the UI (WIMP) point of view.

Also we'd like to avoid "re-inventing the wheel" wherever possible and so we shall reuse (and improve) existsing tools to achieve the goals (where we'll be allowed by the original authors of such tools).

## Project constraints

This is a fully Open Source project and a work of love from the RISC OS community. There is no commercial involvement and/or endorsement. The work is being done when the involved peopel have time and resources and so the major constraints of this project is time.

However the project is open and welcoming everyone that would like to join us and help us.

## Quality control measures

As a fuly Open Source project and a given the contraints above the quality control measures rely on code revies and on the community testing and problems reporting using our Issues Modules.
 

