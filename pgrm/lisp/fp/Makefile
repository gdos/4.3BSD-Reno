#
# Copyright (c) 1987 The Regents of the University of California.
# All rights reserved.
#
# Redistribution and use in source and binary forms are permitted
# provided that the above copyright notice and this paragraph are
# duplicated in all such forms and that any documentation,
# advertising materials, and other materials related to such
# distribution and use acknowledge that the software was developed
# by the University of California, Berkeley.  The name of the
# University may not be used to endorse or promote products derived
# from this software without specific prior written permission.
# THIS SOFTWARE IS PROVIDED ``AS IS'' AND WITHOUT ANY EXPRESS OR
# IMPLIED WARRANTIES, INCLUDING, WITHOUT LIMITATION, THE IMPLIED
# WARRANTIES OF MERCHANTIBILITY AND FITNESS FOR A PARTICULAR PURPOSE.
#
#	@(#)Makefile	5.5 (Berkeley) 3/6/89
#
MAN=	fp.0

all clean depend lint tags: FRC
	cd fp.${MACHINE}; make ${MFLAGS} DESTDIR=${DESTDIR} $@

cleandir: clean
	cd fp.${MACHINE}; make ${MFLAGS} DESTDIR=${DESTDIR} $@
	rm -f ${MAN} tags .depend

install: ${MAN}
	cd fp.${MACHINE}; make ${MFLAGS} DESTDIR=${DESTDIR} $@
	install -c -o bin -g bin -m 444 ${MAN} ${DESTDIR}/usr/man/cat1

FRC:
