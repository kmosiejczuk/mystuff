# $OpenBSD$

COMMENT =		colorize output with xterm 256 color in Python

MODPY_EGG_VERSION =	1.3

DISTNAME =		xtermcolor-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		textproc

HOMEPAGE =		http://github.com/broadinstitute/xtermcolor

MAINTAINER =		Pamela Mosiejczuk <pamela@openbsd.org>

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

FLAVORS =		python3
FLAVOR ?=

NO_TEST =		Yes

post-install:
	mv ${PREFIX}/bin/xtermcolor{,${MODPY_BIN_SUFFIX}}

.include <bsd.port.mk>
