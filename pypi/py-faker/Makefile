# $OpenBSD$

COMMENT =	Faker is a Python package that generates fake data for you

MODPY_EGG_VERSION =	3.0.0

DISTNAME =	Faker-${MODPY_EGG_VERSION}
PKGNAME =	py-${DISTNAME:L}

CATEGORIES =	pypi

HOMEPAGE =	https://github.com/joke2k/faker

# MIT
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

RUN_DEPENDS =		devel/py-dateutil${MODPY_FLAVOR}>=2.4 \
			devel/py-six${MODPY_FLAVOR}>=1.10 \
			net/py-ipaddress \
			pypi/py-text-unidecode${MODPY_FLAVOR}=1.3

FLAVORS =	python3
FLAVOR ?=

.include <bsd.port.mk>
