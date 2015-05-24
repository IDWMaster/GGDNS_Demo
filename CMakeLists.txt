add_executable(distauth GlobalGrid.cpp)
set (EXTRA_LIBS ${EXTRA_LIBS} GlobalGrid)
include_directories(${EXTRA_HEADERS} "${PROJECT_BINARY_DIR}" ".")
target_link_libraries(distauth GlobalGrid uuid fuse rt ${EXTRA_LIBS})
