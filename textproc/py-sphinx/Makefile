# $OpenBSD: Makefile,v 1.25 2019/07/12 20:50:13 sthen Exp $

COMMENT =		python documentation generator

MODPY_EGG_VERSION =	1.8.5
DISTNAME =		Sphinx-${MODPY_EGG_VERSION}
PKGNAME =		py-sphinx-${MODPY_EGG_VERSION}

CATEGORIES =		textproc

HOMEPAGE =		https://www.sphinx-doc.org/

MAINTAINER =		frantisek holop <minusf@obiit.org>

# BSD
PERMIT_PACKAGE =	Yes

MODPY_PI =		Yes

MODULES =		lang/python
RUN_DEPENDS =		devel/py-babel${MODPY_FLAVOR} \
			devel/py-six${MODPY_FLAVOR} \
			graphics/py-imagesize${MODPY_FLAVOR} \
			sysutils/py-packaging${MODPY_FLAVOR} \
			textproc/py-alabaster${MODPY_FLAVOR} \
			textproc/py-docutils${MODPY_FLAVOR} \
			textproc/py-pygments${MODPY_FLAVOR} \
			textproc/py-sphinx_rtd_theme${MODPY_FLAVOR} \
			textproc/py-sphinxcontrib-websupport${MODPY_FLAVOR} \
			textproc/py-snowballstemmer${MODPY_FLAVOR} \
			www/py-jinja2${MODPY_FLAVOR} \
			www/py-requests${MODPY_FLAVOR}
BUILD_DEPENDS =		${RUN_DEPENDS}
TEST_DEPENDS =		devel/py-html5lib${MODPY_FLAVOR} \
			devel/py-mock${MODPY_FLAVOR} \
			print/texlive/texmf,-full

MODPY_SETUPTOOLS =	Yes
MODPY_PYTEST =		Yes

FLAVORS =		python3
FLAVOR ?=

.if !${FLAVOR:Mpython3}
RUN_DEPENDS +=		devel/py-typing
.endif

post-install:
	for i in ${PREFIX}/bin/*; do \
		mv $${i} $${i}${MODPY_BIN_SUFFIX} ;\
	done

.include <bsd.port.mk>
