# $OpenBSD$

COMMENT =		turn CSS blocks into style attributes

MODPY_EGG_VERSION =	3.6.1

DISTNAME =		premailer-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		www

HOMEPAGE =		https://github.com/peterbe/premailer

MAINTAINER =		Pamela Mosiejczuk <pamela@openbsd.org>

# Python Software Foundation license
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes
MODPY_PYTEST_ARGS =	premailer/

FLAVORS =		python3
FLAVOR ?=

RUN_DEPENDS =		devel/py-cachetools${MODPY_FLAVOR} \
			textproc/py-cssselect${MODPY_FLAVOR} \
			textproc/py-cssutils${MODPY_FLAVOR} \
			textproc/py-lxml${MODPY_FLAVOR} \
			www/py-requests${MODPY_FLAVOR}
TEST_DEPENDS =		devel/py-mock${MODPY_FLAVOR} \
			devel/py-nose${MODPY_FLAVOR}

#NO_TEST =		Yes

.include <bsd.port.mk>
