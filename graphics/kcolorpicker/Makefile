# $FreeBSD$

PORTNAME=	kColorPicker
DISTVERSIONPREFIX=	v
DISTVERSION=	0.1.1
CATEGORIES=	graphics kde

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Qt based Color Picker with popup menu

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		cmake qt:5
USE_GITHUB=	yes
GH_ACCOUNT=	ksnip
USE_QT=		core testlib widgets \
		buildtools_build qmake_build

CMAKE_ON=	BUILD_SHARED_LIBS

.include <bsd.port.mk>
