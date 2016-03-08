#  CER Robot test units (Robot Testing Framework)
#  Copyright: (C) 2015 iCub Facility, Istituto Italiano di Tecnologia
#  Authors: Ali Paikan <ali.paikan@gmail.com>
#
#  Copy Policy: Released under the terms of the LGPLv2.1 or later, see LGPL.TXT
#


cmake_minimum_required(VERSION 2.8.9)
project(CER-Tests)

# find a version of RTF higher then 1.0.1
# and with yarp support enabled
find_package(RTF 1.0.1 COMPONENTS YARP REQUIRED)

# set the output plugin directory to collect all the shared libraries
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/plugins)
set(CMAKE_SHARED_MODULE_PREFIX "")

# options
option(CER_TESTS_USES_ICUB_MAIN "Turn on to compile the tests that depend on the icub-main repository" OFF)

# Build example?
#add_subdirectory(example/cpp)


