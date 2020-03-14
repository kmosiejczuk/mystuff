# $OpenBSD$

COMMENT =	debugging manhole for Python applications

MODPY_EGG_VERSION =	1.6.0

DISTNAME =	manhole-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	devel

HOMEPAGE =	https://github.com/ionelmc/python-manhole

# BSD 2-Clause
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =	python3
FLAVOR ?=

TEST_ENV =		TMPDIR=${WRKDIR}

TEST_DEPENDS =		${FULLPKGNAME}:${FULLPKGPATH} \
			devel/py-process-tests${MODPY_FLAVOR}

.include <bsd.port.mk>
