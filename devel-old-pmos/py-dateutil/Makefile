# $OpenBSD: Makefile,v 1.33 2019/12/12 16:21:23 jasper Exp $

COMMENT =		Extensions to the standard Python datetime module

MODPY_EGG_VERSION =	2.8.1
DISTNAME =		python-dateutil-${MODPY_EGG_VERSION}
PKGNAME =		${DISTNAME:S/^python-/py-/}
CATEGORIES =		devel

HOMEPAGE =		https://dateutil.readthedocs.io

# unknown license -> 'Dual License'
PERMIT_PACKAGE =	unknown license

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

BUILD_DEPENDS =		devel/py-setuptools_scm${MODPY_FLAVOR}
RUN_DEPENDS =		devel/py-six${MODPY_FLAVOR}>=1.5
TEST_DEPENDS =		devel/py-freezegun${MODPY_FLAVOR} \
			devel/py-hypothesis${MODPY_FLAVOR} \
			devel/py-six${MODPY_FLAVOR}

FLAVORS =	python3
FLAVOR ?=

# Lines below not in the template
PERMIT_DISTFILES =	unknown license
.include <bsd.port.mk>
