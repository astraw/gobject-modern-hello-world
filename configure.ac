AC_PREREQ(2.65)
AC_INIT([libabc],[0.0.1])

AC_CONFIG_MACRO_DIR([build])
AC_CONFIG_AUX_DIR([build])
AC_CONFIG_SRCDIR([src/abc.h])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE([1.11 dist-bzip2 no-dist-gzip -Wall foreign no-define subdir-objects])

LT_PREREQ([2.2.6])
LT_INIT([])

AC_PROG_CC
AC_HEADER_STDC

AM_SILENT_RULES([yes])

PKG_CHECK_MODULES(DEPS, [gtk+-3.0])
AC_SUBST(DEPS_CFLAGS)
AC_SUBST(DEPS_LIBS)

GOBJECT_INTROSPECTION_CHECK([1.29])

AC_CONFIG_FILES([
Makefile
libabc.pc
])
AC_OUTPUT
