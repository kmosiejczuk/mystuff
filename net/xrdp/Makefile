# $OpenBSD$

COMMENT =		allow RDP connections to your non-windows server

V =			0.9.14
DISTNAME =		xrdp-${V}

SHARED_LIBS +=		common		0.0 # 0.0
SHARED_LIBS +=		scp		0.0 # 0.0
SHARED_LIBS +=		xrdp		0.0 # 0.0
SHARED_LIBS +=		xrdpapi		0.0 # 0.0

CATEGORIES =		net
HOMEPAGE =		http://xrdp.org

MAINTAINER =		Kurt Mosiejczuk <kmos@openbsd.org>

# Apache 2.0
PERMIT_PACKAGE =	Yes

WANTLIB +=		ICE SM X11 Xext Xfixes Xrandr Xrender c crypto
WANTLIB +=		pthread ssl xcb


MASTER_SITES =	https://github.com/neutrinolabs/xrdp/releases/download/v${V}/

AUTOCONF_VERSION =	2.69
AUTOMAKE_VERSION =	1.16

LIB_DEPENDS =		graphics/libpainter \
			graphics/rfxcodec

CONFIGURE_STYLE =	autoreconf
CONFIGURE_ARGS +=	--enable-bsd --disable-painter --disable-rfxcodec

post-install:
	rm ${DESTDIR}/etc/xrdp/*.pem ${DESTDIR}/etc/xrdp/rsakeys.ini
	${INSTALL_DATA_DIR} ${PREFIX}/share/examples/xrdp
	mv ${DESTDIR}/etc/xrdp/* ${PREFIX}/share/examples/xrdp

.include <bsd.port.mk>
