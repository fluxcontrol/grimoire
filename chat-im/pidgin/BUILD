### had to cook up some pkg-config files for nss and nspr 
CFLAGS="$CFLAGS -I${TRACK_ROOT}/usr/X11R6/include" &&

if is_depends_enabled $SPELL gtk+2; then
   LIBS="$LIBS -lX11"
fi &&
export LIBS="${LIBS} -lm" &&

export PKG_CONFIG_PATH="${TRACK_ROOT}/usr/include/nss:${TRACK_ROOT}/usr/include/nspr" &&
make_single          &&
default_build        &&
make_normal          &&
cd $SOURCE_DIRECTORY
