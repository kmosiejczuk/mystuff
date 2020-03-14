# $OpenBSD$

COMMENT =		objects and routines pertaining to date and time

MODPY_EGG_VERSION =	1.14.1
DISTNAME =		tempora-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python
MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

MODPY_PYTEST =		Yes
MODPY_PYTEST_ARGS =	tests/

FLAVORS =		python3
FLAVOR ?=

BUILD_DEPENDS =		devel/py-setuptools_scm${MODPY_FLAVOR}>=1.15.0
RUN_DEPENDS =	 	devel/py-jaraco-functools${MODPY_FLAVOR}>=1.2.0 \
			devel/py-six${MODPY_FLAVOR} \
			devel/py-tz${MODPY_FLAVOR}
TEST_DEPENDS =		devel/flake8 \
			devel/py-freezegun${MODPY_FLAVOR} \
			devel/py-mock${MODPY_FLAVOR}

.if !${FLAVOR:Mpython3}
TEST_DEPENDS +=		devel/py-unittest2
.endif
#NO_TEST =		Yes

post-install:
	mv ${PREFIX}/bin/calc-prorate \
		${PREFIX}/bin/calc-prorate${MODPY_BIN_SUFFIX}

.include <bsd.port.mk>
