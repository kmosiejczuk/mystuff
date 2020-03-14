# $OpenBSD$

COMMENT =	backport of standard library importlib.resources module

MODPY_EGG_VERSION =	1.0.2

DISTNAME =	importlib_resources-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	devel

HOMEPAGE =	http://importlib-resources.readthedocs.io/

# Apache Software License
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

BUILD_DEPENDS =		devel/py-wheel

RUN_DEPENDS =		devel/py-pathlib2 \
			devel/py-typing

.include <bsd.port.mk>
