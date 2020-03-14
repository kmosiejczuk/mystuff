# $OpenBSD$

COMMENT =		backport providing API to access package metadata

MODPY_EGG_VERSION =	1.2.0

DISTNAME =		importlib_metadata-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		http://importlib-metadata.readthedocs.io/

# Apache 2.0
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes
MODPY_PYTEST_ARGS =	importlib_metadata

FLAVORS =		python3
FLAVOR ?=

BUILD_DEPENDS =		devel/py-setuptools_scm${MODPY_FLAVOR}

RUN_DEPENDS =		devel/py-zipp${MODPY_FLAVOR}

TEST_DEPENDS =		sysutils/py-packaging${MODPY_FLAVOR} \
			textproc/py-docutils${MODPY_FLAVOR}

.if ! ${FLAVOR:Mpython3}
RUN_DEPENDS +=		devel/py-configparser \
			devel/py-contextlib2 \
			devel/py-pathlib2

TEST_DEPENDS +=		devel/py-importlib_resources
.endif

.include <bsd.port.mk>
