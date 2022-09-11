idf_component_register(SRCS "mongoose/mongoose.c"
                       INCLUDE_DIRS "mongoose"
                       REQUIRES lwip mbedtls)

target_compile_definitions(${COMPONENT_LIB} PRIVATE MG_ENABLE_MBEDTLS=1)
