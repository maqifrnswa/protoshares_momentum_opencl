#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([FULL-PACKAGE-NAME], [VERSION], [BUG-REPORT-ADDRESS])
AM_INIT_AUTOMAKE([foreign])
AC_CONFIG_SRCDIR([stdafx.cpp])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC

# Checks for libraries.
AC_SEARCH_LIBS([clGetPlatformIDs], [OpenCL],
    [], [AC_MSG_ERROR(OpenCL lib was not found)])

# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h sys/time.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE
AC_TYPE_SIZE_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT64_T
AC_TYPE_UINT8_T

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
AC_CHECK_FUNCS([gettimeofday])

AC_CONFIG_FILES([Makefile])
CXXFLAGS="$CXXFLAGS -std=c++11"
AC_OUTPUT
