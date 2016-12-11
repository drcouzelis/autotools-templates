# SOURCE FILES

# The name of the program to be compiled.
# The "bin" prefix will install it in the "bin" directory.
# The "PROGRAMS" suffix marks it as a program to be compiled.
#
# https://www.gnu.org/software/automake/manual/html_node/Program-Sources.html#Program-Sources
bin_PROGRAMS = myappname

# The "-D" option provides the compiler with a variable
# that points to the location of the data files.
#
# NOTE: "CPP" stands for "C Pre-Processor".
#
# https://www.gnu.org/software/automake/manual/html_node/Program-and-Library-Variables.html
#
# https://www.gnu.org/software/automake/manual/html_node/Uniform.html
myappname_CPPFLAGS = -Wall -Werror -DPKGDATADIR='"$(pkgdatadir)"'

# A list of all of the source code files.
# The "SOURCES" suffix marks it as source code.
#
# https://www.gnu.org/software/automake/manual/html_node/Program-Sources.html#Program-Sources
myappname_SOURCES = \
  src/myappname.c \
  src/myappname.h

# DATA FILES - IMAGES

# Define a new directory.
#
# The "dir" suffix marks this as a directory variable.
#
# The rest of the word (the "not dir" part) becomes
# a Makefile directory variable that can be used in
# other areas.
#
# https://www.gnu.org/software/automake/manual/html_node/Uniform.html
imagesdatadir = $(pkgdatadir)/images

# The "dist" prefix will ensure that these files are
# kept in the distribution release of the package.
#
# The "DATA" suffix marks this as data files for
# the package.
#
# The word inbetween the prefix and suffix must match
# the name of a directory, declared with the suffix
# "dir".
#
# https://www.gnu.org/software/automake/manual/html_node/Data.html
dist_imagesdata_DATA = \
  data/images/my-image-1.png \
  data/images/my-image-2.png

# DATA FILES - SOUNDS

soundsdatadir = $(pkgdatadir)/sounds

dist_soundsdata_DATA = \
  data/sounds/my-sound-1.wav \
  data/sounds/my-sound-2.wav

# SYSTEM FILES

# These files are not installed, but are included when creating a distribution package.
#
# https://www.gnu.org/software/automake/manual/html_node/Basics-of-Distribution.html
EXTRA_DIST = \
  system/myappname.desktop \
  system/myappname.png
