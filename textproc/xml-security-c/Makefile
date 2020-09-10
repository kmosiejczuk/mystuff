# $OpenBSD: Makefile,v 1.19 2020/03/30 11:15:12 fcambus Exp $

COMMENT =	C++ implementation of the primary security standards for XML

DISTNAME =		xml-security-c-2.0.2
CATEGORIES =		textproc devel

SHARED_LIBS +=  	xml-security-c             0.0

HOMEPAGE =		https://santuario.apache.org/index.html

# Apache 2.0
PERMIT_PACKAGE =	Yes

MASTER_SITES =		https://downloads.apache.org/santuario/c-library/

WANTLIB +=		${COMPILER_LIBCXX}

COMPILER =		base-clang ports-gcc

CONFIGURE_STYLE =	gnu
USE_GMAKE =		Yes

CONFIGURE_ARGS +=	--disable-static

RUN_DEPENDS =		textproc/xerces-c
BUILD_DEPENDS =		textproc/xerces-c

post-install:
	rm ${PREFIX}/lib/*.{a,la}

.include <bsd.port.mk>
