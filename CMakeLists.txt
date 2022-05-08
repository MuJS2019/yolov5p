cmake_minimum_required(VERSION 3.4.1)
set(CMAKE_CXX_STANDARD 17)

project(yolov5p6_ncnn)

set(ncnn_DIR ${CMAKE_SOURCE_DIR}/ncnn/lib/cmake/ncnn)
find_package(ncnn REQUIRED)

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable(yolov5p6_ncnn yolov5p6.cpp)

target_link_libraries(
	yolov5p6_ncnn
	${OpenCV_LIBS}
	ncnn
	)
	

	




