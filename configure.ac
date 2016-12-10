# Run "autoreconf --install" to create the "configure" script.

# See here for an explanation of a "configure.ac" file:
#
# https://www.gnu.org/software/automake/manual/html_node/amhello_0027s-configure_002eac-Setup-Explained.html
#
# And here for the entire manual:
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html

# Initialize autoconf with the name of the program,
# the version number, and the contact information.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#Initializing-configure
AC_INIT([myappname], [0.1], [myemailaddress@gmail.com])

# Initialize automake with all warnings.
#
# https://www.gnu.org/software/automake/manual/html_node/Public-Macros.html
#
# "foreign" will ignore any missing files (README, AUTHORS...).
#
# "subdir-objects" will save compiled objects into their original subdirectories.
#
# https://www.gnu.org/software/automake/manual/html_node/Strictness.html
AM_INIT_AUTOMAKE([-Wall -Werror foreign subdir-objects])

# Check for a compiler.
#
# "AC_PROG_CC" for C.
# "AC_PROG_CXX" for C++.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#C-Compiler
AC_PROG_CC

# Check for headers.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#Generic-Headers
AC_CHECK_HEADER([myneededheader.h], [], [AC_MSG_ERROR([myneededheader.h not found.])])

# Check for libraries.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#Libraries
AC_SEARCH_LIBS([a_needed_library_function_name], [myneededlibrary], [], [AC_MSG_ERROR([myneededlibrary not found.])])

# Rebuild these header files.
#
# This header file can be used in the project. It contains
# useful strings provided by Autotools.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#Configuration-Headers
AC_CONFIG_HEADERS([config.h])

# A list of the Makefiles that need to be created.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#Configuration-Files
AC_CONFIG_FILES([Makefile])

# Finish up by writing the new configuration files.
#
# https://www.gnu.org/software/autoconf/manual/autoconf.html#Output
AC_OUTPUT
