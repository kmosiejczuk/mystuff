# $OpenBSD$

COMMENT =		tools to proxy arbitrary(ish) WSGI requests over HTTP

MODPY_EGG_VERSION =	0.4.6

DISTNAME =		WSGIProxy2-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME:L}

CATEGORIES =		www

HOMEPAGE =		https://github.com/gawel/WSGIProxy2/

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

FLAVORS =		python3
FLAVOR ?=

RUN_DEPENDS =		devel/py-six${MODPY_FLAVOR} \
			www/py-webob${MODPY_FLAVOR}
TEST_DEPENDS =		www/py-webtest${MODPY_FLAVOR}

.include <bsd.port.mk>
