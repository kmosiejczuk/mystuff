# $OpenBSD: Makefile,v 1.13 2019/07/12 20:45:54 sthen Exp $

COMMENT =		library for stubbing in Python

MODPY_EGG_VERSION =	2.8.1
DISTNAME =		pytest-cov-${MODPY_EGG_VERSION}
PKGNAME =		${DISTNAME:S/py/py-/}
CATEGORIES =		devel

HOMEPAGE =		https://pytest-cov.readthedocs.org/en/latest/

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

RUN_DEPENDS =		devel/py-coverage${MODPY_FLAVOR} \
			devel/py-test${MODPY_FLAVOR}
TEST_DEPENDS =		devel/py-fields${MODPY_FLAVOR} \
			devel/py-process-tests${MODPY_FLAVOR} \
			devel/py-test-xdist${MODPY_FLAVOR} \
			devel/py-virtualenv${MODPY_FLAVOR}

.include <bsd.port.mk>
