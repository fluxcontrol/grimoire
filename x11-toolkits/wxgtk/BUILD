OPTS="$OPTS
  --enable-optimise
  --disable-debug
  --disable-monolithic
  --enable-shared
  --with-libiconv-prefix=$INSTALL_ROOT/usr
  --enable-geometry
  --enable-unicode
  --enable-graphics_ctx
  --with-gtk=2
" &&
if list_find "$WXGTK_CONTRIB" "xrc"
then
  OPTS="--enable-xrc $OPTS"
fi  &&
default_build &&
for COMPONENT in $WXGTK_CONTRIB; do
  case "$COMPONENT" in
    xrc|animate|mmedia|applet|canvas) continue ;;
  esac &&
  make -C contrib/src/$COMPONENT
done
