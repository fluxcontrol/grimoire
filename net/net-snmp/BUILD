OPTS="$OPTS --with-sys-contact=root@$(hostname -f) \
    --enable-ucd-snmp-compatibility \
    --with-persistent-directory=/var/state/ucd-snmp \
    --with-mib-modules=ucd-snmp/diskio \
    --with-defaults"

make_single &&
default_build &&
make_normal
