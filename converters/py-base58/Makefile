# $OpenBSD$

COMMENT =		base58 implementation

MODPY_EGG_VERSION =	1.0.3

DISTNAME =		base58-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		converters

HOMEPAGE =		https://github.com/keis/base58

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

TEST_DEPENDS =		devel/py-hamcrest${MODPY_FLAVOR}

.include <bsd.port.mk>
