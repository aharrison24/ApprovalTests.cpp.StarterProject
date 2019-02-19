add_library(ApprovalTests INTERFACE)
target_include_directories(ApprovalTests
    SYSTEM INTERFACE
        "${CMAKE_CURRENT_SOURCE_DIR}/include"
)

add_library(ApprovalTests::ApprovalTests ALIAS ApprovalTests)

