# Created by: Torsten Zuehlsdorff <ports@toco-domains.de>
# $FreeBSD$

PORTNAME=	sentry-raven
PORTVERSION=	2.9.0
PORTREVISION=	1
CATEGORIES=	devel rubygems
MASTER_SITES=	RG
PKGNAMESUFFIX=	29

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Client interface for the Sentry error logger

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	rubygem-faraday>=0.7.6<1.0:www/rubygem-faraday

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

PLIST_FILES=	bin/raven29

PORTSCOUT=	limit:^2\.9\.

post-patch:
	@${MV} ${WRKSRC}/exe/raven ${WRKSRC}/exe/raven29

.include <bsd.port.mk>
