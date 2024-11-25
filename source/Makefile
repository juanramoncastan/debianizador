# ----------------------------------------------------------------------
#
#  Copyright (C) 2013 Juan Ramon Castan Guillen <juanramoncastan@yahoo.es>
#    
#  This program is free software; you can redistribute it and/or modify
#  it under the terms of the GNU General Public License as published by
#  the Free Software Foundation; either version 2 of the License, or
#  (at your option) any later version.
#
#  This program is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#  GNU General Public License for more details.
#
# ----------------------------------------------------------------------

# ###########      This is a example of Makefile (toplevel) for debianizador     ###########################
#                   This make file is used only for creating deb package
############################################################################################################
# Version: 1.0-2

# BUILD = "../package-name_version_architecture" given from "debianizador" script
BUILD = ../debpkg
PREFIX = /usr/local
#SRC_PATH = /source
BIN_PATH = /bin
#SHARE_PATH = /share

test:
	@ echo "This is the first order in makefile"
	@ echo ">$ make (without order)"

install: 
ifneq ($(PREFIX),)
	mkdir -p $(BUILD)$(PREFIX)$(BIN_PATH)
	cp .$(BIN_PATH)/* $(BUILD)$(PREFIX)$(BIN_PATH)
endif

clean:
	rm $(BUILD)$(PREFIX)$(BIN_PATH)
