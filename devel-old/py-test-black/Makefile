# $OpenBSD$

COMMENT =	pytest plugin to enable format checking with black

MODPY_EGG_VERSION =	0.3.7

DISTNAME =	pytest-black-${MODPY_EGG_VERSION}
PKGNAME =	${DISTNAME:S/py/py-/}

CATEGORIES =	devel

HOMEPAGE =	https://github.com/shopkeep/pytest-black

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =	python3
FLAVOR ?=

BUILD_DEPENDS =		devel/py-setuptools_scm${MODPY_FLAVOR}
RUN_DEPENDS =		textproc/py-black \
			textproc/py-toml${MODPY_FLAVOR}
.include <bsd.port.mk>
