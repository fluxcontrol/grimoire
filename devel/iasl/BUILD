CFLAGS="${CFLAGS/-Wunsafe-loop-optimizations}" &&
cd generate/unix &&

make_single  &&
if [[ ${SMGL_COMPAT_ARCHS[1]} == "x86_64" ]]; then
  make BITS=64 HOST=_LINUX iasl
else
  make BITS=32 HOST=_LINUX iasl
fi &&
make_normal
