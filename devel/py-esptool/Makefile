# $OpenBSD$

COMMENT =		esp8266 and esp32 rom bootloader communication tool

MODPY_EGG_VERSION =	2.8
DISTNAME =		esptool-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}


CATEGORIES =		devel
HOMEPAGE =		https://github.com/espressif/esptool

#GPLv2
PERMIT_PACKAGE =	Yes

MODULES =		lang/python
RUN_DEPENDS +=		devel/py-serial${MODPY_FLAVOR} \
			security/py-aes${MODPY_FLAVOR} \
			security/py-ecdsa${MODPY_FLAVOR} \

NO_TEST =		Yes

MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}
MODPY_PI =		Yes
MODPY_SETUPTOOLS =      Yes

.include <bsd.port.mk>
