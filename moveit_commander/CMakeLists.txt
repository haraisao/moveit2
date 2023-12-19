cmake_minimum_required(VERSION 3.22)
project(moveit_commander)

#find_package(ament_cmake REQUIRED)
find_package(PythonInterp REQUIRED)
find_package(PythonLibs "${PYTHON_VERSION_MAJOR}.${PYTHON_VERSION_MINOR}" REQUIRED)

set(PYTHON_LIB_DESTINATION "local/lib/python${PYTHON_VERSION_MAJOR}.${PYTHON_VERSION_MINOR}/dist-packages")

install(DIRECTORY src/ DESTINATION ${PYTHON_LIB_DESTINATION})

#add_subdirectory(test)

