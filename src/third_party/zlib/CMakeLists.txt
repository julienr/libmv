PROJECT(zlib)

ADD_DEFINITIONS(-D_CRT_SECURE_NO_WARNINGS)

ADD_LIBRARY(zlib
  adler32.c    compress.c   crc32.c      deflate.c    gzio.c       infback.c
  inffast.c    inflate.c    inftrees.c   minigzip.c   trees.c      uncompr.c
  zutil.c      crc32.h      deflate.h    inffast.h    inffixed.h   inflate.h
  inftrees.h   trees.h      zconf.h      zconf.in.h   zlib.h       zutil.h
)

LIBMV_INSTALL_THIRD_PARTY_LIB(zlib)
