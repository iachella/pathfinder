cmake_minimum_required(VERSION 3.13)
project(PathFinder)

set(CMAKE_CXX_STANDARD 20)
add_compile_options(
        # -Wcast-align
        # -Wpedantic
        # -Wcast-qual
        # -Wconversion
        # -Wctor-dtor-privacy
        # -Wnon-virtual-dtor
        # -Wmissing-include-dirs
        # -Wdisabled-optimization
        # -Winit-self
        # -Wnon-virtual-dtor
        # -Wold-style-cast
        # -Woverloaded-virtual
        # -Wparentheses
        # -Wredundant-decls
        # -Wshadow
        # -Wsign-promo
        # -Wstrict-aliasing
        # -Wall
        # -Wextra
        # -Werror
)
set(smartcar_test ${CMAKE_CURRENT_SOURCE_DIR}/arduino/wrappers)

add_subdirectory(external)
enable_testing()
add_subdirectory(test)
