# $OpenBSD$

COMMENT =		sphinx API for Web Apps

MODPY_EGG_VERSION =	1.1.2

DISTNAME =		sphinxcontrib-websupport-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		textproc www

HOMEPAGE =		https://github.com/sphinx-doc/sphinxcontrib-websupport

# BSD
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

TEST_DEPENDS =		devel/py-mock${MODPY_FLAVOR} \
			devel/py-six${MODPY_FLAVOR} \
			textproc/py-docutils${MODPY_FLAVOR} \
			textproc/py-sphinx${MODPY_FLAVOR} \
			www/py-jinja2${MODPY_FLAVOR}

FLAVORS =		python3
FLAVOR ?=

.include <bsd.port.mk>
