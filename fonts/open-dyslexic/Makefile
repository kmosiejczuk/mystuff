# $OpenBSD: Makefile.template,v 1.85 2019/09/09 19:19:05 kmos Exp $

COMMENT =	font to increase readability for readers with dyslexia

GH_ACCOUNT =	antijingoist
GH_PROJECT =	opendyslexic
GH_TAGNAME =	v0.9.10

CATEGORIES =	fonts

HOMEPAGE =	https://opendyslexic.org

MAINTAINER =	Pamela Mosiejczuk <pamela@openbsd.org>

# SIL OFL 1.1
PERMIT_PACKAGE =	Yes

NO_BUILD =		Yes
NO_TEST =		Yes

FONTDIR =		${PREFIX}/share/fonts/open-dyslexic
DOCDIR =		${PREFIX}/share/doc/open-dyslexic

do-install:
	${INSTALL_DATA_DIR} ${FONTDIR} ${DOCDIR}
	${INSTALL_DATA} ${WRKDIST}/compiled/{*.otf,*.woff} ${FONTDIR}
	${INSTALL_DATA} ${WRKDIST}/{OFL.txt,OFL-FAQ.txt,README.md} ${DOCDIR}

.include <bsd.port.mk>
