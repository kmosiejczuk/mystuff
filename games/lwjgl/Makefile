# $OpenBSD: Makefile,v 1.10 2019/09/23 15:17:35 kurt Exp $

COMMENT=	lightweight game library for java

V=		3.2.3
GH_ACCOUNT=	kmosiejczuk
GH_PROJECT=	lwjgl3
GH_TAGNAME=	${V}-openbsd
DISTNAME=	lwjgl3-${V}
PKGNAME=	lwjgl-${V}

.if ${MACHINE_ARCH} == "i386"
M_ARCH=		""
.elif ${MACHINE_ARCH} == "amd64"
M_ARCH=		64
.endif

LWJGL_HOME=	${PREFIX}/share/lwjgl

CATEGORIES=	games devel

HOMEPAGE=	https://lwjgl.org

MAINTAINER=	Aaron Bieber <abieber@openbsd.org>

COMPILERS=	base-clang ports-gcc

# BSD
PERMIT_PACKAGE=	Yes

# GL listed here as it is dlopen()d by the lib
WANTLIB +=	${COMPILER_LIBCXX} GL X11 Xcursor Xext Xrandr Xxf86vm m pthread

MODULES=	java
MODJAVA_VER=	1.8
MODJAVA_BUILD=	ant

LIB_DEPENDS=	archivers/lz4 \
		archivers/zstd \
		audio/openal \
		audio/opus \
		databases/lmdb \
		devel/bullet \
		graphics/glfw \
		multimedia/assimp \
		sysutils/xxhash

NO_TEST=	Yes

SUBST_VARS+=	M_ARCH

pre-configure:
	perl -pi -e 's,/usr/X11R6,${X11BASE},g' \
		${WRKSRC}/platform_build/bsd_ant/build.xml
	perl -pi -e 's,/usr/local,${LOCALBASE},g' \
		${WRKSRC}/platform_build/bsd_ant/build.xml

do-install:
	${INSTALL_DATA_DIR} ${LWJGL_HOME}
	for x in ${WRKSRC}/libs/*.jar; do \
		${INSTALL_DATA} $$x ${LWJGL_HOME}/; \
	done
	${INSTALL_DATA} ${WRKSRC}/libs/openbsd/liblwjgl${M_ARCH}.so ${LWJGL_HOME}/

.include <bsd.port.mk>