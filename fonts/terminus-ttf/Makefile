# $OpenBSD$

COMMENT =		TTF version of terminus

VERSION =	4.47.0
DISTNAME =	terminus-ttf-${VERSION}
EXTRACT_SUFX =	.zip

HOMEPAGE=	https://files.ax86.net/terminus-ttf/
MASTER_SITES =	https://files.ax86.net/terminus-ttf/files/${VERSION}/

CATEGORIES=	fonts x11

# OFL 1.1
PERMIT_PACKAGE=	Yes

NO_BUILD=	Yes
NO_TEST=	Yes

PKG_ARCH=	*

FONTDIR=	${PREFIX}/share/fonts/terminus-ttf
FONTS =	"TerminusTTF-Bold Italic" TerminusTTF-Italic TerminusTTF TerminusTTF-Bold


do-install:
	${INSTALL_DATA_DIR} ${FONTDIR} ${DOCDIR}
.for f in ${FONTS}
	${INSTALL_DATA} ${WRKDIST}/${f}-${VERSION}.ttf ${FONTDIR}/${f}.ttf
.endfor

.include <bsd.port.mk>
