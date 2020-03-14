# $OpenBSD$

COMMENT =		subprocesses for humans 2.0

MODPY_EGG_VERSION =	0.1.1

DISTNAME =		delegator.py-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://github.com/kennethreitz/delegator

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

RUN_DEPENDS =		devel/py-pexpect${MODPY_FLAVOR}

FLAVORS =		python3
FLAVOR ?=

.include <bsd.port.mk>
