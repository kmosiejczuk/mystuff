# $OpenBSD$

COMMENT =		library for working with color names and color values

MODPY_EGG_VERSION =	1.10

DISTNAME =		webcolors-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		www

HOMEPAGE =		https://github.com/ubernostrum/webcolors

MAINTAINER =		Pamela Mosiejczuk <pamela@openbsd.org>

# BSD 3-Clause
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

RUN_DEPENDS =		devel/py-six${MODPY_FLAVOR}

FLAVORS =		python3
FLAVOR ?=

TEST_ENV +=		PYTHONPATH=${WRKSRC}/src

.include <bsd.port.mk>
