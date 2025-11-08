cmake_minimum_required(VERSION 3.20)

project(chibicc LANGUAGES C)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/output)

add_executable(chibicc
    codegen.c
    hashmap.c
    main.c
    parse.c
    preprocess.c
    strings.c
    tokenize.c
    type.c
    unicode.c
)

target_include_directories(chibicc
PUBLIC
    .
)