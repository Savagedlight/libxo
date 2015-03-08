# $FreeBSD: head/usr.bin/iscsictl/Makefile 275510 2014-12-05 12:38:01Z trasz $

PROG=		iscsictl
SRCS=		iscsictl.c periphs.c parse.y token.l y.tab.h
CFLAGS+=	-I${.CURDIR}
CFLAGS+=	-I${.CURDIR}/../../sys/dev/iscsi
MAN=		iscsi.conf.5 iscsictl.8

LIBADD=		cam util
LDADD=		-lxo

YFLAGS+=	-v
LFLAGS+=	-i
CLEANFILES=	y.tab.c y.tab.h y.output

WARNS=		6
NO_WMISSING_VARIABLE_DECLARATIONS=

.include <bsd.prog.mk>
