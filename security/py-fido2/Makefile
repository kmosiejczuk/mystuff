# $OpenBSD: Makefile.template,v 1.85 2019/09/09 19:19:05 kmos Exp $

COMMENT =		provides library functionality for FIDO 2.0

MODPY_EGG_VERSION =	0.7.3

DISTNAME =		fido2-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		security sysutils

HOMEPAGE =		https://github.com/Yubico/python-fido2

# BSD
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

RUN_DEPENDS =		devel/py-six${MODPY_FLAVOR} \
			security/py-cryptography${MODPY_FLAVOR}
TEST_DEPENDS =		devel/py-mock${MODPY_FLAVOR}

.include <bsd.port.mk>
