#	@(#)Makefile	7.12 (Berkeley) 5/24/90

PROG=	newfs
CFLAGS+=-DMFS
SRCS=	newfs.c mkfs.c
MAN8=	newfs.0
LINKS=	${BINDIR}/newfs ${BINDIR}/mount_mfs
MLINKS=	newfs.8 mfs.8

.include <bsd.prog.mk>
