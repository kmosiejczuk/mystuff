# $OpenBSD$

COMMENT =		run a test with multiple data sets

MODPY_EGG_VERSION =	1.3.2

DISTNAME =		genty-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://github.com/box/genty

# Apache 2.0
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

RUN_DEPENDS =		devel/py-mock${MODPY_FLAVOR} \
			devel/py-six${MODPY_FLAVOR}

FLAVORS =		python3
FLAVOR ?=

.include <bsd.port.mk>
