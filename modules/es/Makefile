#---------------------------------------------------------------------------------
.SUFFIXES:
#---------------------------------------------------------------------------------
ifeq ($(SDKDIR),)
export SDKDIR = $(CURDIR)/../../sdk
endif

include $(SDKDIR)/starstruck_rules

#---------------------------------------------------------------------------------
# TARGET is the name of the output
# BUILD is the directory where object files & intermediate files will be placed
# SOURCES is a list of directories containing source code
# INCLUDES is a list of directories containing extra header files
# DATA is a list of directories containing binary data
#
# All directories are specified relative to the project directory where
# the makefile is found
#
#---------------------------------------------------------------------------------
SOURCES			:= source $(wildcard source/*/)
INCLUDES		:= source
DATA			:=
PROCESSID		:= 0x01
PRIORITY		:= 0x79
VIRTUALADDR		:= 0x20100000
PHYSADDR		:= 0x139F0000
STACKSIZE		:= 0x4000

include $(SDKDIR)/modules.mk
