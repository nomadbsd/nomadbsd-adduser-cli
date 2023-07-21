# CREATING THE BINARY APP FILE
add_executable(nadduser nomadbsd-adduser.c)

#GCC OPTIONS
target_compile_options(nadduser PRIVATE
    -Wall
    -Wextra
    -Wpedantic
    -Werror
    -O2
    -g
    -std=c17
    -pthread
    -fstrict-aliasing
    -fstack-protector-strong
    -fno-strict-overflow
    -fno-delete-null-pointer-checks
    -fvisibility=hidden
    -Wformat=2
    -Wstrict-overflow=5
    -Wcast-align
)

# LINK THE LIBRARIES
#target_link_libraries(nadduser nadduser-messages)