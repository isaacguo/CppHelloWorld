project(cpphelloworld CXX)
cmake_minimum_required(VERSION 2.6.2)

include_directories(
	${CalcComponent_SOURCE_DIR}/include
	)


add_executable(cpphelloworld src/cpphelloworld.cpp)

target_link_libraries(cpphelloworld pthread)

install(TARGETS cpphelloworld DESTINATION bin)

