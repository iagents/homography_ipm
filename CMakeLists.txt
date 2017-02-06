##############################
PROJECT( ipm )
##############################
cmake_minimum_required (VERSION 2.6)

# Packages
find_package(OpenCV REQUIRED)

# Includes
include_directories( include	
	${OPENCV_INCLUDE_DIR}
	${PROJECT_BINARY_DIR}
)

#set(SOURCE_FILES 
#	main.cpp
#	IPM.cpp
#	IPM.h
#)
file(GLOB SOURCE_FILES "src/*.cpp")

# Add executable and target link libraries
ADD_EXECUTABLE(ipm ${SOURCE_FILES})
TARGET_LINK_LIBRARIES(ipm ${OpenCV_LIBS})


