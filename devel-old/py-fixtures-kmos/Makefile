# $OpenBSD$

COMMENT =		reusable state for writing clean tests and more

MODPY_EGG_VERSION =	3.0.0

DISTNAME =		fixtures-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://launchpad.net/python-fixtures

# BSD and Apache 2.0
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}

BUILD_DEPENDS =		devel/py-pbr${MODPY_FLAVOR}
TEST_DEPENDS =		devel/py-testtools${MODPY_FLAVOR}

.include <bsd.port.mk>
