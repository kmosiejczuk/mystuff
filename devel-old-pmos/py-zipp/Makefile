# $OpenBSD$

COMMENT =	backport of pathlib-compatible object wrapper for zip files

MODPY_EGG_VERSION =	0.6.0

DISTNAME =		zipp-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://github.com/jaraco/zipp

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

BUILD_DEPENDS =		devel/py-setuptools_scm${MODPY_FLAVOR}
RUN_DEPENDS =		devel/py-more-itertools${MODPY_FLAVOR}
TEST_DEPENDS =		devel/py-contextlib2${MODPY_FLAVOR} \
			devel/py-pathlib2${MODPY_FLAVOR} \

.if ! ${FLAVOR:Mpython3}
TEST_DEPENDS +=		devel/py-unittest2
.endif

.include <bsd.port.mk>
