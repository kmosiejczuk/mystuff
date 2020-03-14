# $OpenBSD$

COMMENT =	Async generators and context managers for Python 3.5+

MODPY_EGG_VERSION =	1.10

DISTNAME =	async_generator-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	devel

HOMEPAGE =	https://github.com/python-trio/async_generator

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}
MODPY_PYTEST =		Yes
MODPY_PYTEST_ARGS =	async_generator/_tests

.include <bsd.port.mk>
