# Build dependency
add_subdirectory(lib/libxbee-v3)
include_directories(lib/libxbee-v3)

set(src
  in_xbee.c in_xbee_config.c in_xbee_iosampling.c in_xbee_utils.c)

FLB_PLUGIN(in_xbee "${src}" "xbee")
