cmake_minimum_required (VERSION 2.8) 

PROJECT(Cartoonifier_Desktop)
set (OpenCV_DIR "C:/opencv_build")
# Requires OpenCV
FIND_PACKAGE( OpenCV REQUIRED )

SET(SRC
    main_desktop.cpp
    cartoon.cpp
    ImageUtils_0.7.cpp
)

ADD_EXECUTABLE( ${PROJECT_NAME} ${SRC} )
TARGET_LINK_LIBRARIES( ${PROJECT_NAME}  ${OpenCV_LIBS} )
