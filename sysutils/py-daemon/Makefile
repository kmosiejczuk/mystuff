# $OpenBSD: Makefile,v 1.10 2019/07/12 20:49:49 sthen Exp $

COMMENT=		library to implement a Unix daemon process

MODPY_EGG_VERSION=	2.2.3
DISTNAME=		python-daemon-${MODPY_EGG_VERSION}
PKGNAME=		py-daemon-${MODPY_EGG_VERSION}

CATEGORIES=		sysutils


# PSF-2+
PERMIT_PACKAGE=		Yes

MODULES=		lang/python

MODPY_PI=		Yes
MODPY_SETUPTOOLS=	Yes

FLAVORS=		python3
FLAVOR?=

BUILD_DEPENDS=		textproc/py-docutils${MODPY_FLAVOR}
RUN_DEPENDS=		sysutils/py-lockfile${MODPY_FLAVOR}
TEST_DEPENDS=		textproc/py-docutils${MODPY_FLAVOR}

.if !${FLAVOR:Mpython3}
TEST_DEPENDS+=		devel/py-mock
.endif

post-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/doc/py-daemon/
	${INSTALL_DATA} ${WRKSRC}/doc/FAQ ${PREFIX}/share/doc/py-daemon/

.include <bsd.port.mk>
