#cmake_minimum_required(VERSION 3.8)
#project(StarterProject.tests)
#set(CMAKE_CXX_STANDARD 17)

add_executable(StarterProject.tests
    main.cpp
    DemoTest.cpp
    NewTest.cpp
)

target_link_libraries(StarterProject.tests
    PRIVATE
        StarterProject.code
        ApprovalTests::ApprovalTests
        Catch::Catch
)

add_test(NAME StarterProject.tests COMMAND StarterProject.tests)
