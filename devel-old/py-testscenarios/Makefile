# $OpenBSD$

COMMENT =		pyunit extension for dependency injection

MODPY_EGG_VERSION =	0.5.0

DISTNAME =		testscenarios-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://launchpad.net/testscenarios

# BSD 3-clause or Apache 2.0
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

FLAVORS =		python3
FLAVOR ?=

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes
MODPY_PYTEST_ARGS =	testscenarios

BUILD_DEPENDS =		devel/py-pbr${MODPY_FLAVOR}
TEST_DEPENDS =		${FULLPKGNAME}:${FULLPKGPATH} \
			devel/py-testtools${MODPY_FLAVOR}

#TEST_ENV =		PYTHONPATH=.

.include <bsd.port.mk>
