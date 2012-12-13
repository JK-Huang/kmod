PROG = kmod

SRCS = depmod.c  insmod.c  kmod.c  log.c  lsmod.c  modinfo.c  modprobe.c  rmmod.c

.for x in ls rm ins dep
LINKS += kmod ${x}mod
.endfor

.for x in info probe
LINKS += kmod mod${x}
.endfor

LDADD += ../libkmod/libkmod.a

.include <bsd.prog.mk>
