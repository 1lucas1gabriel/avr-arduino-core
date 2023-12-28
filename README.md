# avr-arduino-core

**avr-arduino-core** allows the usage of arduino core libraries with AVR microcontrollers. It can be used to setup quick avr workspaces to work with handy arduino implementation in low cost devices. The repository includes automated Makefiles to quick building for any arduino supported target. By default AVR-ARDUINO-CORE was already pre-compiled to generate a static library (.a file) targeting the ATMEGA328P. This device target can be changed and re-compiled to generate a new static library under the Makefile.incl. Use the Makefile within the template folder to link the Core library with the source files from your project.

## Folder description
- **cores:** Includes a copy of arduino core folder, where resides main src files implementing well-known arduino functions. 
- **variants:** Includes pinouts files for each arduino supported board.
- **template:** Includes .cpp src file and Makefile as an easy-to-start example.

## Dependencies
To use AVR-ARDUINO-CORE some tools are required to be pre-installed on your host PC.
- GCC-AVR Toolchain (gcc-avr, binutils-avr, avr-libc)
- AVRDUDE
- MAKE
