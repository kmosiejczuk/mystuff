# $OpenBSD$

COMMENT =	command line tools to provide basic accessibility validation

MODPY_EGG_VERSION =	0.2.6

DISTNAME =		wcag-zoo-${MODPY_EGG_VERSION}
PKGNAME =		${DISTNAME}

CATEGORIES =		www

HOMEPAGE =		https://github.com/data61/wcag-zoo

MAINTAINER =		Pamela Mosiejczuk <pamela@openbsd.org>

# BSD
PERMIT_PACKAGE =	Yes

MODULES =		lang/python

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}

RUN_DEPENDS =		devel/py-click${MODPY_FLAVOR} \
			textproc/py-lxml${MODPY_FLAVOR} \
			textproc/py-xtermcolor${MODPY_FLAVOR} \
			www/py-webcolors${MODPY_FLAVOR} \
			www/py-premailer${MODPY_FLAVOR}

.include <bsd.port.mk>
