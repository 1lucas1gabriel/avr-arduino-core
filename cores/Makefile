######################################################################
#  Project Makefile - Arduino Core for ATMEGA328p
######################################################################

ARCHIVE		= 	core_atmega328p
SRCFILES	= 	wiring_pulseASM.S \
			WInterrupts.c hooks.c wiring.c wiring_analog.c wiring_digital.c wiring_pulse.c wiring_shift.c \
			CDC.cpp HardwareSerial.cpp HardwareSerial0.cpp HardwareSerial1.cpp HardwareSerial2.cpp HardwareSerial3.cpp \
			IPAddress.cpp PluggableUSB.cpp Print.cpp Stream.cpp Tone.cpp USBCore.cpp WMath.cpp WString.cpp abi.cpp new.cpp

# wiring_pulse.S changed to wiring_pulseASM.S to avoid overwriting c file (wiring_pulse.c)
# main.cpp removed from core -> needs to declared main function and include Arduino.h under the project source code

# Dependecies Directory (Header Files)
INCLUDES	+= -I$(TOP_DIR)/cores
INCLUDES	+= -I$(TOP_DIR)/variants/standard

# search a way to execute core and clean automatically
all: lib clean


# DEPS		= 	# Any additional dependencies for your build
# CLOBBER	+= 	# Any additional files to be removed with "make clobber"

include ../Makefile.incl

######################################################################
#  NOTES:
#	1. remove any modules you don't need from SRCFILES
#	2. "make clean" will remove *.o etc., but leaves *.elf, *.bin
#	3. "make clobber" will "clean" and remove *.elf, *.bin etc.
######################################################################
