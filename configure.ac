AC_PREREQ([2.68])
AC_INIT([websocketpp], [0.2.0], [jonathan.rosser@rd.bbc.co.uk])

AM_INIT_AUTOMAKE([1.11 silent-rules])
AM_SILENT_RULES([yes])
AM_MAINTAINER_MODE([enable])

WSPP_MAJORMINOR=0.2
AC_SUBST(WSPP_MAJORMINOR)

dnl CURRENT, REVISION, AGE
dnl - library source changed -> increment REVISION
dnl - interfaces added/removed/changed -> increment CURRENT, REVISION = 0
dnl - interfaces added -> increment AGE
dnl - interfaces removed -> AGE = 0
WSPP_LIBVERSION="1:0:0"
AC_SUBST(WSPP_LIBVERSION)

AC_CONFIG_MACRO_DIR([m4])
ACLOCAL_AMFLAGS="-I m4 $ACLOCAL_AMFLAGS"
AC_SUBST(ACLOCAL_AMFLAGS)

LT_PREREQ([2.2.6])
LT_INIT(disable-static)

AC_PROG_CXX
AM_PROG_CC_C_O

AC_CONFIG_SRCDIR([src/common.hpp])
AC_CONFIG_HEADERS([config.h])

AX_BOOST_BASE([1.48.0], HAVE_BOOST=yes, HAVE_BOOST=no)
if test "x${HAVE_BOOST}" != xyes ; then
  AC_MSG_ERROR(Boost library is required)
fi
AX_BOOST_DATE_TIME
AX_BOOST_PROGRAM_OPTIONS
AX_BOOST_REGEX
AX_BOOST_SYSTEM
AX_BOOST_UNIT_TEST_FRAMEWORK
AX_BOOST_THREAD
AX_BOOST_RANDOM
AX_BOOST_CHRONO

SSL_VER="1.0.1"
PKG_CHECK_MODULES(SSL, openssl >= $SSL_VER, HAVE_SSL=yes, HAVE_SSL=no)
if test "x${HAVE_SSL}" != xyes ; then
  AC_ERROR([openssl >= $SSL_VER is required])
fi
WSPP_LIB_DEPS="$WSPP_LIB_DEPS $SSL_LIBS"

AX_CREATE_STDINT_H([src/websocketpp-stdint.h])

WSPP_CFLAGS="$WSPP_CFLAGS -I\$(top_srcdir)"
AC_SUBST(WSPP_CFLAGS)

WSPP_LIBS="\$(top_builddir)/src/libwebsocketpp-$WSPP_MAJORMINOR.la"
AC_SUBST(WSPP_LIBS)

AC_SUBST(WSPP_LIB_DEPS)
AC_SUBST(WSPP_PKG_DEPS)

pkgconfigdir="\$(libdir)/pkgconfig"
AC_SUBST(pkgconfigdir)

AC_CONFIG_FILES([Makefile
                   src/Makefile
                   test/basic/Makefile
                   examples/Makefile
		   examples/broadcast_server_tls/Makefile
                   examples/chat_client/Makefile
                   examples/chat_server/Makefile
		   examples/concurrent_server/Makefile
                   examples/echo_client/Makefile
                   examples/echo_server/Makefile
		   examples/echo_server_tls/Makefile
		   examples/fuzzing_client/Makefile
		   examples/fuzzing_server_tls/Makefile
		   examples/stress_client/Makefile
		   examples/telemetry_server/Makefile
		   examples/wsperf/Makefile
		   websocketpp.pc
])
AC_OUTPUT
