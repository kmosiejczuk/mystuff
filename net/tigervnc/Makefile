# $OpenBSD: Makefile.template,v 1.86 2019/11/19 12:39:04 espie Exp $

COMMENT =		high-performance, platform-neutral VNC

V =			1.10.1

CATEGORIES =		net

GH_ACCOUNT =		TigerVNC
GH_PROJECT =		tigervnc
GH_TAGNAME =		v${V}

HOMEPAGE =		https://tigervnc.org

MAINTAINER =		Florian Viehweger <openbsd@out-of-creativity.de>

# unsure here
PERMIT_PACKAGE =	Yes

#WANTLIB =		X11

MODULES =		devel/cmake

# Dependencies
LIB_DEPENDS =		archivers/libzip \
			graphics/jpeg \
			x11/fltk

BUILD_DEPENDS =		devel/gettext,-tools \
			devel/nasm

.include <bsd.port.mk>
