add_library(puzzleFetcher)

target_include_directories(puzzleFetcher PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/inc
    ${CMAKE_CURRENT_SOURCE_DIR}/src
)

target_sources(puzzleFetcher PUBLIC src/puzzleFetcher.cpp)