# Abstract Microcontroller Handlers

Microcontroller development platforms (MPLAB from Microchip, CodeWarrior from NXP, and so on) may have utilities to generate code (`.c` and `.h` files... maybe `.o`). Implementing solutions around these `.h` files may lead to code that won't be able to be ported to other microcontrollers.

Here I propose this library with "abstract" headers (`.h` files) of peripherals, so it can be used against (if possible) most of these platforms, to keep portable the code, relying only in platform specific implementations of these headers.

## Usage

Create a `.c` file (maybe based from one in the [examples folder](examples/)) that implements the `.h` header file you need. Configure your project to include the [src folder](src/) as it includes the "abstract" headers.
