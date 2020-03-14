# $OpenBSD$

COMMENT =		backport importlib.resources to pythons before 3.7

MODPY_EGG_VERSION =	1.0.2

DISTNAME =		importlib_resources-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://importlib-resources.readthedocs.io/

# Apache Software License
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes
MODPY_PYTEST_ARGS =	importlib_resources/

BUILD_DEPENDS =		devel/py-wheel

RUN_DEPENDS =		devel/py-pathlib2 \
			devel/py-typing

.include <bsd.port.mk>
