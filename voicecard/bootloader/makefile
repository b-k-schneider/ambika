# Copyright 2011 Olivier Gillet.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

VERSION        = 0.1
MCU_NAME       = 328
TARGET         = ambika_voicecard_boot
PACKAGES       = avrlib voicecard/bootloader
EXTRA_DEFINES  = -funsigned-char -fno-inline-small-functions
EXTRA_LD_FLAGS = ,--section-start=.text=0x7e00,--relax -nostartfiles

LFUSE          = ff
HFUSE          = de
EFUSE          = fd
LOCK           = 2f

include avrlib/makefile.mk

include $(DEP_FILE)
