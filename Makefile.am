ACLOCAL_AMFLAGS = -I m4
AM_DISTCHECK_CONFIGURE_FLAGS = --enable-tests

if ENABLE_TESTS
MAYBE_OPT = tests
endif

SUBDIRS = noinst src $(MAYBE_OPT)
DIST_SUBDIRS = noinst src $(MAYBE_OPT)

debian-package:
	dpkg-buildpackage -rfakeroot -tc -us -uc
