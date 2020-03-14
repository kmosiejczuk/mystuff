# $OpenBSD$

COMMENT =		retrieve and read MLB GameDay data

MODPY_EGG_VERSION =	2.5.0

DISTNAME =		mlbgame-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		misc

HOMEPAGE =		https://github.com/zachpanz88/mlbgame

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}

RUN_DEPENDS =		textproc/py-lxml${MODPY_FLAVOR}

.include <bsd.port.mk>
