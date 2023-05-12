add_executable(app test.cpp)

target_link_libraries(app Catch2::Catch2WithMain)

list(APPEND INCLUDES ${CMAKE_SOURCE_DIR}/src)
list(APPEND INCLUDES ${CMAKE_SOURCE_DIR}/src/third_party)

target_include_directories(app PUBLIC ${INCLUDES})
