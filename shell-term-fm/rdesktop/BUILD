OPTS="$RDESKTOP_IPV6  \
      --without-libvncserver \
      $OPTS"          &&

if  [  "$RDESKTOP_SOUND"  !=  "none"  ];  then
  OPTS="--with-sound=$RDESKTOP_SOUND  \
        $OPTS"
fi  &&

default_build
