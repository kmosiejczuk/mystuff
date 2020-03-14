# $OpenBSD$

COMMENT =		multi-library, cross-platform audio decoding

MODPY_EGG_VERSION =	2.1.8

DISTNAME =		audioread-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		audio

HOMEPAGE =		https://github.com/sampsyo/audioread

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

BUILD_DEPENDS =		devel/py-test-runner${MODPY_FLAVOR}

# Tests are broken in tarball for 2.1.8
NO_TEST =		Yes

.include <bsd.port.mk>
