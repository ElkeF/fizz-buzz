add_library(
    fizz_buzz
    SHARED
    fizz_buzz.f90
    fizz_buzz.h
    divisible.f90
    )

add_executable(
    fb.x
    main.cpp
    )

target_link_libraries(
    fb.x
    fizz_buzz
    )
