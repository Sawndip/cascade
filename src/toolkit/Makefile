#
#    Automatically Generated Makefile Include
#    Sat Nov 14 17:19:04 EST 2015
#
#
#    Configured for Darwin

CC=cc
MACHDEP_CFLAGS=-Ofast
#  	C Function Toolkit
#  	Makefile
#
#  	V1.0
#	Matt White (mwhite+@cmu.edu)
#	10/2/94


CFLAGS= $(MACHDEP_CFLAGS) -O
OBJS= memory.o prompt.o string.o str_cvrt.o queue.o vector.o vectori.o

libtoolkit.a:	$(OBJS)
	        rm -f libtoolkit.a
		ar r libtoolkit.a $(OBJS)
		ranlib libtoolkit.a

memory.o:	memory.c toolkit.h
prompt.o:       prompt.c toolkit.h
string.o:	string.c memory.c toolkit.h
str_cvrt.o:     str_cvrt.c toolkit.h

queue.o:	queue.c queue.h toolkit.h
vector.o:	vector.c vector.h
vectori.o:	vectori.c vector.h

install:	libtoolkit.a toolkit.h vector.h queue.h
		'cp' libtoolkit.a $(INSTALL_DIR)/lib
		'cp' toolkit.h $(INSTALL_DIR)/include
		'cp' vector.h $(INSTALL_DIR)/include
		'cp' queue.h $(INSTALL_DIR)/include

clean:
		rm -f *.o *.u *~ core
