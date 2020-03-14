# $OpenBSD$

COMMENT =	Query metadatdata from sdists / bdists / installed packages

MODPY_EGG_VERSION =	1.5.0.1

DISTNAME =	pkginfo-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME}

CATEGORIES =	pypi

HOMEPAGE =	https://code.launchpad.net/~tseaver/pkginfo/trunk

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

TEST_DEPENDS =		devel/py-coverage${MODPY_FLAVOR} \
			devel/py-nose${MODPY_FLAVOR}

FLAVORS =	python3
FLAVOR ?=

.include <bsd.port.mk>
