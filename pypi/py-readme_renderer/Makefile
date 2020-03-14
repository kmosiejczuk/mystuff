# $OpenBSD$

COMMENT =	readme_renderer is a library for rendering "readme"

MODPY_EGG_VERSION =	24.0

DISTNAME =	readme_renderer-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	pypi

HOMEPAGE =	https://github.com/pypa/readme_renderer

# Apache 2.0
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

RUN_DEPENDS =		devel/py-six${MODPY_FLAVOR} \
			pypi/py-cmarkgfm${MODPY_FLAVOR}>=0.2.0 \
			textproc/py-docutils${MODPY_FLAVOR}>=0.13.1 \
			textproc/py-pygments${MODPY_FLAVOR} \
			www/py-bleach${MODPY_FLAVOR}>=2.1.0

FLAVORS =	python3
FLAVOR ?=

.include <bsd.port.mk>
