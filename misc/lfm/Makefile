# $OpenBSD: Makefile,v 1.7 2019/07/17 14:46:33 danj Exp $

COMMENT =		powerful curses interface python file manager

MODPY_EGG_VERSION =	3.1
DISTNAME =		lfm-${MODPY_EGG_VERSION}

CATEGORIES =		misc

HOMEPAGE =		https://katxi.org/devel/lfm/

# GPLv3+
PERMIT_PACKAGE =	Yes

MODPY_PI =		Yes

MODULES =		lang/python
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}

NO_TEST =		Yes

post-install:
		${INSTALL_MAN} ${WRKSRC}/lfm.1 ${PREFIX}/man/man1

.include <bsd.port.mk>
