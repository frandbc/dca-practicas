AC_INIT([tporo],[1.0])
AC_CONFIG_SRCDIR(lib/tporo.cpp)
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])

AC_PROG_RANLIB
AM_PROG_AR

AM_INIT_AUTOMAKE(foreign)

AM_SILENT_RULES([yes])
AM_PROG_AR

AC_PROG_CXX
AC_PROG_CC

AC_DEFUN([acb_BOOST_TEST],
			[AC_MSG_CHECKING([for boost::test])
			 AC_LANG_PUSH([C++])
			 AC_CHECK_HEADER([boost/test/unit_test.hpp],,
			 AC_MSG_WARN([Boost header unit_test.hpp not found. Can't generate test suite.]))
			 AC_LANG_POP()
			]
		)
acb_BOOST_TEST

AC_CONFIG_FILES([Makefile
include/Makefile
lib/Makefile
test-cxxtest/Makefile
test-boost/Makefile])

AC_OUTPUT
