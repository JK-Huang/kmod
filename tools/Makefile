PROG = kmod

SRCS = depmod.c  insmod.c  kmod.c  log.c  lsmod.c  modinfo.c  modprobe.c  rmmod.c

MAN  = depmod.d.5 modprobe.d.5 modules.dep.5 depmod.8 insmod.8 lsmod.8 rmmod.8 modprobe.8 modinfo.8

.for x in ls rm ins dep
LINKS += kmod ${x}mod
.endfor

.for x in info probe
LINKS += kmod mod${x}
.endfor

CFLAGS += -I../libkmod -include ../config.h
LDADD  += ../libkmod/libkmod.a -lz -llzma

.include <bsd.prog.mk>
