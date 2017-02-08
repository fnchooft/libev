AC_INIT(libev,4.22.1,[],libev,[http://github.com/fnchooft/libev])
AC_CONFIG_SRCDIR([ev_epoll.c])
AM_INIT_AUTOMAKE

orig_CFLAGS="$CFLAGS"


dnl also update ev.h!
AC_CONFIG_HEADERS([config.h])
AM_MAINTAINER_MODE

AC_PROG_CC

dnl Supply default CFLAGS, if not specified
if test -z "$orig_CFLAGS"; then
  if test x$GCC = xyes; then
    CFLAGS="-g -O3"
  fi
fi

AC_PROG_INSTALL
AC_PROG_LIBTOOL

m4_include([libev.m4])

AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([$PACKAGE_NAME.pc:pc.in])
AC_OUTPUT
