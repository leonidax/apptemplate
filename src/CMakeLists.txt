include_directories(${CMAKE_SOURCE_DIR}/include)

add_library( ${LIB_NAME}
    AppCore.cpp
)

add_executable( ${APP_NAME}
    # Add source files here
    main.cpp
)

target_link_libraries( ${APP_NAME}
    # Add libraries here
    ${LIB_NAME}
)
