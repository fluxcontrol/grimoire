#message CFLAGS=$CFLAGS
OPTS+=" xorg=$XSERVER_XORG \
        xwayland=$XSERVER_WAYLAND \
        xnest=$XSERVER_XNEST \
        xvfb=$XSERVER_XVFB \
        xephyr=$XSERVER_XEPHYR \
        dmx=$XSERVER_DMX \
        xkb_bin_dir=$INSTALL_ROOT/usr/bin \
        os_vendor='SourceMage'"
PREFIX=/opt/xorg &&
#PREFIX=/usr &&
check_tmp_noexec /tmp &&
default_build &&
check_tmp_noexec /tmp
