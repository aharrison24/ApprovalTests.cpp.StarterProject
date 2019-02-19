add_library(Catch INTERFACE)
target_include_directories(Catch
    SYSTEM INTERFACE
        "${CMAKE_CURRENT_SOURCE_DIR}/include"
)

add_library(Catch::Catch ALIAS Catch)

