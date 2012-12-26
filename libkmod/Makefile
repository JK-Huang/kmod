SUBDIR = util

LIB = kmod

SRCS = libkmod.c libkmod-list.c libkmod-config.c libkmod-index.c libkmod-module.c libkmod-file.c libkmod-elf.c

CFLAGS += -include ../config.h

libkmod.a: util

.include <bsd.lib.mk>
