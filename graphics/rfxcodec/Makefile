# $OpenBSD$

COMMENT =		JPEG2000 codec for RDP

V =			0.1.5
DISTNAME =		rfxcodec-${V}

SHARED_LIBS +=		rfxencode	0.0

CATEGORIES =		graphics
HOMEPAGE =		http://xrdp.org

MAINTAINER =		Kurt Mosiejczuk <kmos@openbsd.org>

# Apache 2.0
PERMIT_PACKAGE =	Yes

MASTER_SITES =	https://github.com/neutrinolabs/librfxcodec/releases/download/v${V}/

AUTOCONF_VERSION =	2.69
AUTOMAKE_VERSION =	1.16

BUILD_DEPENDS =		devel/yasm

CONFIGURE_STYLE =	autoreconf

.include <bsd.port.mk>
