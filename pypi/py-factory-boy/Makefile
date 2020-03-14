# $OpenBSD$

COMMENT =	versatile test fixtures replacement based on thoughtbot's

MODPY_EGG_VERSION =	2.12.0

DISTNAME =	factory_boy-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	pypi

HOMEPAGE =	https://github.com/FactoryBoy/factory_boy

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

RUN_DEPENDS =		pypi/py-faker${MODPY_FLAVOR}>=0.7.0

FLAVORS =	python3
FLAVOR ?=

.include <bsd.port.mk>
