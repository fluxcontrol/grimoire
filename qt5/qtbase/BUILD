
OPTS="$QT_DEBUG               \
      $QT_DECL                \
      $QT_GIF                 \
      $QT_PCH                 \
      $QT_EXAMPLE examples    \
      $QT_TESTS tests         \
      $QT_ACCESS              \
      $OPTS"                  &&
cd $SOURCE_DIRECTORY &&

./configure  -opensource -confirm-license \
             -prefix $QT5DIR  -platform  linux-g++  \
             -reduce-relocations -reduce-exports $OPTS -v &&
make

