# $FreeBSD$

PORTNAME=	clixon
PORTVERSION=	4.4.0
CATEGORIES=	devel

MAINTAINER=	dcornejo@netgate.com
COMMENT=	YANG-based toolchain including CLI, NETCONF and RESTCONF interfaces

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE.md

LIB_DEPENDS=	libcligen.so:devel/cligen \
		libfcgi.so:www/fcgi
BUILD_DEPENDS=	cligen>=4.4.0:devel/cligen

USES=		autoreconf bison compiler:c11 gmake

USE_LDCONFIG=	yes
USE_GITHUB=	yes

GH_ACCOUNT=	clicon
MAKE_ARGS=	wwwdir=${PREFIX}/sbin \
		wwwuser=${WWWOWN}

GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--sysconfdir=${ETCDIR} \
		--with-cligen=${LOCALBASE}
CONFIGURE_ENV=	YACC="bison -y"

SUB_FILES=	pkg-message

.include <bsd.port.mk>
