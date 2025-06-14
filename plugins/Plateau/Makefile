#!/usr/bin/make -f
# Makefile for DISTRHO Plugins #
# ---------------------------- #
# Created by falkTX
#
# Modified by REIS0
# Modified by lamech
# Modified by dreamer

# --------------------------------------------------------------
# Project name, used for binaries

NAME = Plateau

# --------------------------------------------------------------
# Files to build

FILES_DSP = PlateauPlugin.cpp

FILES_UI = PlateauUI.cpp \
widgets/StaticImageBase.cpp \

# --------------------------------------------------------------
# Do some magic

UI_TYPE = cairo
include ../../dpf/Makefile.plugins.mk

# --------------------------------------------------------------
# PLugin targets

TARGETS += vst2
TARGETS += vst3
TARGETS += lv2_sep
TARGETS += clap
TARGETS += au

check:
	@echo "Building targets: $(TARGETS)"

all: check $(TARGETS)

art: # Converts the artwork to a header file
	python ../../dpf/utils/png2rgba.py PlateauArtwork artwork
