######################################################################
#  Project Makefile - Template Project
######################################################################

BINARY		= main
SRCFILES	= template.cpp

# Dependencies directory (Header Files)
#INCLUDES	+= -I$(TOP_DIR)/template	#template.h
INCLUDES	+= -I$(TOP_DIR)/cores
INCLUDES	+= -I$(TOP_DIR)/variants/standard

# Dependencies Directory (Static Libs Folder)
LDFLAGS		+= -L$(TOP_DIR)/cores

# Dependencies (Static Lib Files .a)
LDLIBS		+= -lcore_atmega328p	#last


all: hex clean


# DEPS		= 	# Any additional dependencies for your build
# CLOBBER	+= 	# Any additional files to be removed with "make clobber"

include ../Makefile.incl

######################################################################
#  NOTES:
#	1. remove any modules you don't need from SRCFILES
#	2. "make clean" will remove *.o etc., but leaves *.elf, *.bin
#	3. "make clobber" will "clean" and remove *.elf, *.bin etc.
######################################################################
