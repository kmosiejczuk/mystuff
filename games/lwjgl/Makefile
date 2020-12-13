# $OpenBSD: Makefile,v 1.10 2019/09/23 15:17:35 kurt Exp $

COMMENT=	lightweight game library for java

V=		3.2.3
GH_ACCOUNT=	kmosiejczuk
GH_PROJECT=	lwjgl3
GH_TAGNAME=	openbsd-working
DISTNAME=	lwjgl3-${V}
PKGNAME=	lwjgl3-${V}

.if ${MACHINE_ARCH} == "i386"
M_ARCH=		""
.elif ${MACHINE_ARCH} == "amd64"
M_ARCH=		64
.endif

LWJGL3_HOME=	${PREFIX}/share/lwjgl3

CATEGORIES=	games devel

HOMEPAGE=	https://lwjgl.org

COMPILERS=	base-clang ports-gcc

# BSD
PERMIT_PACKAGE=	Yes

# GL listed here as it is dlopen()d by the lib
WANTLIB +=	${COMPILER_LIBCXX} GL X11 Xcursor Xext Xrandr Xxf86vm m pthread
WANTLIB +=	gtk-3

MODULES=	java
MODJAVA_VER=	11
MODJAVA_BUILD=	ant
MODJAVA_BUILD_TARGET_NAME=	compile-templates \
				compile \
				compile-native \
				release

LIB_DEPENDS=	archivers/lz4 \
		archivers/zstd \
		audio/openal \
		audio/opus \
		databases/lmdb \
		devel/bullet \
		devel/dyncall \
		graphics/glfw \
		multimedia/assimp \
		sysutils/xxhash \
		x11/gtk+3

NO_TEST=	Yes

SUBST_VARS+=	M_ARCH

#
# This is a crude temporary hack. Left to its own devices, the build will
# download a fresh copy of the 1.3.50 version of the Kotlin compiler. If
# You unzip that in your home directory and change "kurt" to your user,
# this will symbolic link in and save yourself a sizable download each time
# you build via this port.
#
# (The mkdir and ln -s. The perl substitution stuff is a more normal
#  part of the port)
#
pre-configure:
	perl -pi -e 's,/usr/X11R6,${X11BASE},g' \
		${WRKSRC}/config/openbsd/build.xml
	perl -pi -e 's,/usr/local,${LOCALBASE},g' \
		${WRKSRC}/config/openbsd/build.xml
	mkdir -p ${WRKSRC}/bin/libs
	ln -s /home/kurt/kotlinc ${WRKSRC}/bin/libs/

do-install:
	${INSTALL_DATA_DIR} ${LWJGL3_HOME}
	for x in ${WRKSRC}/bin/libs/java/*.jar; do \
		${INSTALL_DATA} $$x ${LWJGL3_HOME}/; \
	done
	for x in ${WRKSRC}/bin/libs/native/openbsd/x64/org/lwjgl/*/*.so; do \
		${INSTALL_DATA} $$x ${LWJGL3_HOME}/; \
	done
	${INSTALL_DATA} ${WRKSRC}/bin/libs/native/openbsd/x64/org/lwjgl/liblwjgl.so ${LWJGL3_HOME}/

.include <bsd.port.mk>
