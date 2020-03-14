# $OpenBSD$

COMMENT =	Hunter is a flexible code tracing toolkit

MODPY_EGG_VERSION =	3.0.4

DISTNAME =	hunter-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	pypi

HOMEPAGE =	https://github.com/ionelmc/python-hunter

# unknown license -> 'BSD-2-Clause'
PERMIT_PACKAGE =	unknown license
PERMIT_DISTFILES =	unknown license

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

RUN_DEPENDS =		devel/py-colorama${MODPY_FLAVOR} \
			pypi/py-manhole${MODPY_FLAVOR}>=1.5

FLAVORS =	python3
FLAVOR ?=

.include <bsd.port.mk>
