project(test_signal)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} ${Boost_LIBRARIES}
                                      ${ZeroMQ_LIBRARIES}
                                      ${CMAKE_THREAD_LIBS_INIT})

add_catch_test(${PROJECT_NAME})
