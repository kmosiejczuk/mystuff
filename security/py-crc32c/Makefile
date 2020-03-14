# $OpenBSD$

COMMENT =		implementatation of the crc32c algorithm

MODPY_EGG_VERSION =	2.0

DISTNAME =		crc32c-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		security

HOMEPAGE =		https://github.com/ICRAR/crc32c

MAINTAINER =		Kurt Mosiejczuk <kmos@openbsd.org>

# LGPLv2.1+
PERMIT_PACKAGE =	yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

TESTLIBDIR =		${WRKSRC}/lib.openbsd-${OSREV}-${ARCH}-${MODPY_VERSION}
TEST_ENV +=		PYTHONPATH=${TESTLIBDIR}

.include <bsd.port.mk>
