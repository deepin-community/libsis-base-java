MBO=$(shell if [ `dpkg-architecture -qDEB_BUILD_ARCH_ENDIAN` = little ] ; then echo 1 ; else echo 2; fi )
AM_CFLAGS=-I/usr/lib/jvm/default-java/include -I/usr/lib/jvm/default-java/include/linux -DMACHINE_BYTE_ORDER=$(MBO)

lib_LTLIBRARIES = libcisd_unix.la libcisd_nativedata.la
libcisd_unix_la_SOURCES = unix.c
#libcisd_unix_la_LD_FLAGS = 
libcisd_nativedata_la_SOURCES = copyByteChar.c copyByteDouble.c copyByteFloat.c copyByteInt.c copyByteLong.c copyByteShort.c copyCommon.c
#libcisd_nativedata_la_LDFLAGS = -DMACHINE_BYTE_ORDER=1
