# $OpenBSD$

COMMENT =		Python bindings for MPI

MODPY_EGG_VERSION =	3.0.3

DISTNAME =		mpi4py-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}

CATEGORIES =		devel

SHARED_LIBS +=		dl		0.0

HOMEPAGE =		https://bitbucket.org/mpi4py/mpi4py/

# BSD
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

#WANTLIB =		MPI dl
WANTLIB =		mpi dl

FLAVORS =		python3
FLAVOR ?=

LIB_DEPENDS =		devel/openmpi

TEST_ENV =		PYTHONPATH=${WRKSRC}/src/

.include <bsd.port.mk>
