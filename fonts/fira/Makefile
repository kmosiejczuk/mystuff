# $OpenBSD: Makefile,v 1.9 2019/07/12 20:46:11 sthen Exp $

COMMENT =		Firefox OS typeface

V =			4.202
PKGNAME =		fira-${V}

GH_ACCOUNT =		mozilla
GH_PROJECT =		fira
GH_TAGNAME =		${V}

CATEGORIES =		fonts x11

# SIL OFL 1.1
PERMIT_PACKAGE =	Yes

NO_BUILD =		Yes
NO_TEST =		Yes

PKG_ARCH =		*

WRKDIST =		${WRKDIR}/Fira-${V}

FONTDIR =		${PREFIX}/share/fonts/fira
DOCDIR =		${PREFIX}/share/doc/fira

do-install:
	${INSTALL_DATA_DIR} ${FONTDIR} ${DOCDIR}
	${INSTALL_DATA} ${WRKDIST}/otf/*.otf ${FONTDIR}
	${INSTALL_DATA} ${WRKDIST}/ttf/*.ttf ${FONTDIR}
	${INSTALL_DATA} ${WRKDIST}/woff/*.woff ${FONTDIR}
	${INSTALL_DATA} ${WRKDIST}/woff2/*.woff2 ${FONTDIR}
	${INSTALL_DATA} ${WRKDIST}/{LICENSE,README.md} ${DOCDIR}

.include <bsd.port.mk>
