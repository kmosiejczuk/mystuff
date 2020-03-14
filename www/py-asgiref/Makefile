# $OpenBSD$

COMMENT =		base libraries for Async Server Gateway Interface

MODPY_EGG_VERSION =	3.2.2

DISTNAME =		asgiref-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		www devel

HOMEPAGE =		http://github.com/django/asgiref/

MAINTAINER =		Wen Heping <wenheping2000@hotmail.com>

# BSD
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}
MODPY_PYTEST =		Yes

# Tests aren't bundled on PyPI yet
# Will need pytest-asyncio for most tests

.include <bsd.port.mk>
