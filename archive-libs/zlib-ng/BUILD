cd "$SOURCE_DIRECTORY"  &&
mkdir -p build        &&
cd build              &&
prepare_cmake_flags   &&

CMAKE_INSTALL_PREFIX="$INSTALL_ROOT/usr"

message INSTALL_PREFIX=$CMAKE_INSTALL_PREFIX &&

cmake -DCMAKE_INSTALL_PREFIX=$CMAKE_INSTALL_PREFIX \
      -DCMAKE_INSTALL_LIBDIR="$INSTALL_ROOT"/lib \
      -DCMAKE_INSTALL_MANDIR=share/man \
      -DCMAKE_PREFIX_PATH=share/apps/cmake/modules \
      -DSYSCONFDIR="$INSTALL_ROOT"/etc \
      -DCMAKE_BUILD_TYPE=Release \
      -DCMAKE_C_FLAGS_RELEASE="$CFLAGS" \
      -DCMAKE_CXX_FLAGS_RELEASE="$CXXFLAGS" \
       $OPTS ../  &&
make
