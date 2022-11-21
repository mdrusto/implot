project(implot LANGUAGES CXX)

set(IMPLOT_DIR ${CMAKE_CURRENT_SOURCE_DIR})
add_library(implot STATIC)

target_sources(implot PRIVATE ${IMPLOT_DIR}/implot_demo.cpp ${IMPLOT_DIR}/implot_items.cpp ${IMPLOT_DIR}/implot.cpp)

target_include_directories(implot PUBLIC ${IMPLOT_DIR})

target_link_libraries(implot PUBLIC imgui)
