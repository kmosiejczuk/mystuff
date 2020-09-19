# $OpenBSD$
#
COMMENT =		library for manipulating memory bitmaps

V =			0.1.1
DISTNAME =		libpainter-${V}

SHARED_LIBS +=		painter		0.0

CATEGORIES =		graphics
HOMEPAGE =		http://xrdp.org

MAINTAINER =		Kurt Mosiejczuk <kmos@openbsd.org>

# Apache 2.0
PERMIT_PACKAGE =	Yes

# "make port-lib-depends-check" can help
#WANTLIB =		???

MASTER_SITES =	https://github.com/neutrinolabs/libpainter/releases/download/v${V}/

AUTOCONF_VERSION =	2.69
AUTOMAKE_VERSION =	1.16

# Dependencies
#BUILD_DEPENDS =	???
#RUN_DEPENDS =		???
#LIB_DEPENDS =		???
#TEST_DEPENDS =		???

CONFIGURE_STYLE =	autoreconf
#CONFIGURE_ARGS +=	--enable-bsd

.include <bsd.port.mk>
