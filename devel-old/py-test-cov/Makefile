# $OpenBSD: Makefile,v 1.13 2019/07/12 20:45:54 sthen Exp $

COMMENT =		Pytest plugin for measuring coverage

MODPY_EGG_VERSION =	2.8.1
DISTNAME =		pytest-cov-${MODPY_EGG_VERSION}
PKGNAME =		${DISTNAME:S/py/py-/}
CATEGORIES =		devel

HOMEPAGE =		https://github.com/pytest-dev/pytest-cov

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

RUN_DEPENDS =		devel/py-coverage${MODPY_FLAVOR}>=4.4 \
			devel/py-test${MODPY_FLAVOR}>=3.6

TEST_DEPENDS =		devel/py-six${MODPY_FLAVOR} \
			devel/py-virtualenv${MODPY_FLAVOR} \
			pypi/py-fields${MODPY_FLAVOR} \
			pypi/py-hunter${MODPY_FLAVOR} \
			pypi/py-process-tests=2.0.2

.include <bsd.port.mk>
