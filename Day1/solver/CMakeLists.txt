add_library(solver)

target_include_directories(solver PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/inc
    ${CMAKE_CURRENT_SOURCE_DIR}/src
)

target_sources(solver PUBLIC src/solver.cpp)