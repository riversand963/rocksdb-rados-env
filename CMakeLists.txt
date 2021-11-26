cmake_minimum_required(VERSION 3.4)

# Requires librados.
# https://docs.ceph.com/en/latest/rados/api/librados-intro/ does not mention
# Windows as supported platform, nor does it explain how to get librados on
# Windows. The document does list a few other operating systems.
# https://github.com/AcalephStorage/rados_dll is a Windows port of librados.
# Windows support is not available in this plugin.

set(rados_SOURCES env_librados.cc PARENT_SCOPE)
set(rados_LIBS rados PARENT_SCOPE)
