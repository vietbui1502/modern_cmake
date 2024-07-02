set(LIBRARY_SOURCES
    "my_lib.cc")
set(LIBRARY_HEADERS
    "my_lib.h")

add_library(${LIBARY_NAME} STATIC 
    ${LIBRARY_SOURCES}
    )
target_include_directories(${LIBARY_NAME} PUBLIC 
    "./"
    ${CMAKE_BINARY_DIR}/configured_files)