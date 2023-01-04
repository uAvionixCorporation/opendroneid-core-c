idf_component_register(SRCS "libopendroneid/opendroneid.c" "libopendroneid/wifi.c"
                    INCLUDE_DIRS "libopendroneid")
					
target_compile_options(${COMPONENT_LIB} PRIVATE "-Wno-format")
target_compile_options(${COMPONENT_LIB} PRIVATE "-D_FORTIFY_SOURCE=2")
target_compile_options(${COMPONENT_LIB} PRIVATE "-fstack-protector")
target_compile_options(${COMPONENT_LIB} PRIVATE "-fno-delete-null-pointer-checks")
target_compile_options(${COMPONENT_LIB} PRIVATE "-fwrapv")
target_compile_options(${COMPONENT_LIB} PRIVATE "-O0")
target_compile_options(${COMPONENT_LIB} PRIVATE "-Wall")
target_compile_options(${COMPONENT_LIB} PRIVATE "-Wdouble-promotion")
target_compile_options(${COMPONENT_LIB} PRIVATE "-Wno-address-of-packed-member")
target_compile_options(${COMPONENT_LIB} PRIVATE "-Wextra")
