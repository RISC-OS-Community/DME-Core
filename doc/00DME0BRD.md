# Business Requirements Document

## Project overview

One of the first elements of a Modern Operating System (OS) that is perceived by any type of user is the usability of its interaction environment (either command line or graphical user interface based).

Regardless of the technologies implied in the general architecture of the OS or the number of applications it can be used for, how we can interact with it is the very first element a user will always perceive.

On top of that the user interface (UI) can also make (or break) the productivity that an OS offers to users of every type.

Finally in modern times general (and non general) users are exposed to a lot of different OS compared to what used to happen back in the early days of home computing pioneers and so they have developed expectations and perceptions towards how such UI interaction should happen.

So far, RISC OS has received little to none improvement and refactoring to follow the new trends on the matter of UI and this can cause two sorts of problems:

a) New users may perceive RISC OS as difficult or not intuitive (according to the new perceptions described above)
b) RISC OS may not be as customisable and offer an enjoyable experience as much as other OS can do these days

So we thought it would be very useful to introduce a way to allow such changes to be applicable to the RISC OS UI in order to improve and facilitate new users experience on our beloved OS.

At the same time such changes shall not be invasive and shall be kept optional for the userbase that prefers the original way RISC OS has to interact with the user.

RISC OS Desktop and its users would benefit from:
- A customizable desktop through the addition of a powerful and easy to use Theme Manager
- More modern and useful functionalities like 
  - Introducing instant desktop notifications via a new configurable framework
  - Fast features access via a new global keyboard shortcuts framework
  - Essential keyboard control of the mouse pointer (for those situations where the mouse may abbandon us!)
  - and more 

## Success factors

We'd define as success factors for this project:
- The possibility for a new user to define and use an environment and UI as close as possible to "the modern perceptions created by far more popular OS like MS Windows and Apple macOS". While users acustomed to the old UI shall be let free to keep using the OS as they liked it to be.
- An extremely easy way to achieve their UI configuration goals that would require little to no knowledge of RISC OS for the new users and little to no knowledge of the new UI from experienced users.
- All the changes and improvements would reside in a single and easy to install (and remove) "Package". 

## Project Scope

This project has no intention to modify the OS internals. In a first phase it should be limited to work to add the required tools to achieve the goals in the overview and, eventually, in a second phase it may be sligthely more *invasive*, but only from the UI (WIMP) point of view.

Also we'd like to avoid "re-inventing the wheel" wherever possible and so we shall reuse (and improve) existsing tools to achieve the goals (where we'll be allowed by the original authors of such tools).

## Project constraints

This is a fully Open Source project and a work of love from the RISC OS community. There is no commercial involvement and/or endorsement. The work is being done when the involved people have time and resources and so the major constraints of this project is time.

However the project is open and welcoming everyone that would like to join us and help us.

## Quality control measures

As a fully Open Source project and given the contraints above the quality control measures, this project relies on code reviews and community testing and problem reporting using our Issues Modules (in github).
 
