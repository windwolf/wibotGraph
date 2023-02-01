cmake_minimum_required(VERSION 3.14 FATAL_ERROR)


add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/u8g2)
process_src_dir(${CMAKE_CURRENT_LIST_DIR}/u8g2/cppsrc ${PROJECT_NAME})

target_link_libraries(${PROJECT_NAME} PRIVATE u8g2)
