# $OpenBSD$

COMMENT =		utilities for publishing packages on PyPI

MODPY_EGG_VERSION =	3.1.0

DISTNAME =		twine-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://twine.readthedocs.io/

# Apache 2.0
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}
MODPY_PYTEST =		Yes

BUILD_DEPENDS =		devel/py-setuptools_scm${MODPY_FLAVOR}
TEST_DEPENDS =		net/py-portend${MODPY_FLAVOR} \
			www/py-requests${MODPY_FLAVOR}

.include <bsd.port.mk>
