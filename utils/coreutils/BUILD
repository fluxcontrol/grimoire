FORCE_UNSAFE_CONFIGURE=1 ./configure       \
   --build=$BUILD                          \
   --bindir=${TRACK_ROOT}/bin              \
   --prefix=${TRACK_ROOT}/usr              \
   --mandir=${TRACK_ROOT}/usr/share/man    \
   --infodir=${TRACK_ROOT}/usr/share/info  \
   $SELINUX                                \
   $OPTS                                   &&

make_single                                &&
make  $MAKEFLAG DESTDIR=$INSTALL_ROOT      &&
make_normal
