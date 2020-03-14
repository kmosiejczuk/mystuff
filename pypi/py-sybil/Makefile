# $OpenBSD$

COMMENT =		automated testing for the examples in your docs

MODPY_EGG_VERSION =	1.2.0

DISTNAME =		sybil-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

HOMEPAGE =		https://github.com/cjw296/sybil

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

BUILD_DEPENDS =		devel/py-setuptools_git${MODPY_FLAVOR} \
			devel/py-wheel${MODPY_FLAVOR} \
			pypi/py-pkginfo${MODPY_FLAVOR} \
			pypi/py-twine \
			textproc/py-sphinx${MODPY_FLAVOR}
TEST_DEPENDS =		devel/py-nose${MODPY_FLAVOR} \
			devel/py-test${MODPY_FLAVOR}>=3.5.0 \
			devel/py-test-cov${MODPY_FLAVOR}

FLAVORS =	python3
FLAVOR ?=

.include <bsd.port.mk>
